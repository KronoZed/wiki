title: Scrot
category: Связанное с десктопом
---
### Scrot - утилита командной строки для снятия скриншотов.

##### сделать скриншот в текущей директории с именем, которое по умолчанию имеет формат date-time_resolution_scrot.png:
```
scrot
```

##### этот параметр заснимет ещё и обрамление окна:
```
-b, --border
```

##### количество секунд, через которое будет сделан снимок:
```
-d, --delay NUM
```

##### отображение обратного отсчёта:
```
-c, --count
```

##### этот параметр позволяет выполнить дополнительную команду:
```
-e, --exec APP
```

##### возможность регулировки качества изображения. Диапазон от 1 до 100. По-умолчанию 75:
```
-q, --quality NUM
```

##### этот параметр позволяет сделать снимок нужного окна просто кликнув мышкой на нём:
```
-s, --select
```

##### этот параметр позволяет сделать снимок активного окна:
```
-u, --focused
```

##### этот параметр позволяет сделать миниатюру вместе со снимком экрана. В качестве значения NUM принимается число. Расчет производится в процентах от оригинального размера:
```
-t, --thumb NUM
```

##### специальные значения можно использовать для подстановки значений в параметр --exec или имя файла:
* $f — путь/имя изображения (игнорируется, если используется в имени файла)
* $m — путь/имя эскиза
* $n — имя изображения (игнорируется, если используется в имени файла)
* $s — размер изображения (в байтах) (игнорируется, если используется в имени файла)
* $p — размер изображения в пикселях
* $w — ширина изображения
* $h — высота изображения
* $t — формат изображения
* $$ — выводит символ '$'
* \n — перевод строки (игнорируется, если используется в имени файла)

##### перенос снимка в другую директорию:
```
scrot '%Y-%m-%d_%H-%M-%S_$wx$h.png' -e 'mv $f ~/Картинки/screenshots/'
```

##### вывод оповещения:
```
scrot '%Y-%m-%d_%H-%M-%S_$wx$h.png' -e 'mv $f ~/Картинки/screenshots/ && notify-send "Скриншот сделан и перенесён в папку ~/Картинки/screenshots/"'
```

##### выбор окна:
```
#!/bin/sh
sleep 0.2 ; scrot -s '%Y-%m-%d_at_%I:%M:%S_$wx$h.png' -e 'mv $f ~/Картинки/screenshots && notify-send "Скриншот сделан и перенесён в папку ~/Картинки/screenshots/"'
```

##### скрипт автоснимков:
```
#!/bin/bash
while true;
do
scrot -d 5 -q 50 '%Y-%m-%d_%H-%M-%S.jpg' -e 'mv $f ~/Картинки/screenshots/';
done
```

##### скрипт заливки скриншота на удалённый примонтированный раздел:
```
#!/bin/bash

if [[ -n "$*" ]]; then
    FILENAME="$*"
else
    FILENAME="$(date +'%Y-%m-%d_at_%H-%M-%S')_$HOSTNAME.png"
fi

if  scrot -q 100 ~/share/root.kronoz.guru/screenshots/${FILENAME} ; then
    notify-send -u low -t 1500 "Скриншот ${FILENAME} сделан и загружен на сервер root.kronoz.guru"

    URI="http://root.kronoz.guru/screenshots/${FILENAME}"
    echo -n $URI | tee >(xclip) && echo

    chromium http://root.kronoz.guru/screenshots/${FILENAME}
else
    notify-send -u critical -t 3000 "Не удалось сделать скриншот"
fi

exit
```
##### скрипт выбора окна и заливки скриншота на удалённый примонтированный раздел:
```
#!/bin/bash

if [[ -n "$*" ]]; then
    FILENAME="$*"
else
    FILENAME="$(date +'%Y-%m-%d_at_%H-%M-%S')_$HOSTNAME.png"
fi

if  sleep 0.2 ; scrot -s -q 100 ~/share/root.kronoz.guru/screenshots/${FILENAME} ; then
    notify-send -u low -t 1500 "Скриншот ${FILENAME} сделан и загружен на сервер root.kronoz.guru"

    URI="http://root.kronoz.guru/screenshots/${FILENAME}"
    echo -n $URI | tee >(xclip) && echo

    chromium http://root.kronoz.guru/screenshots/${FILENAME}
else
    notify-send -u critical -t 3000 "Не удалось сделать скриншот"
fi

exit
```