title: gentoo-overlay
category: My projects
#### Установка
Вариант 1:
Выполните:
```
layman -f -o https://raw.githubusercontent.com/KronoZed/gentoo-overlay/master/repositories.xml -a kronoz
```
Вариант 2:
Чтобы добавить его в список layman`a, откройте /etc/layman/layman.cfg и сразу после строки:
```
overlays  : http://www.gentoo.org/proj/en/overlays/repositories.xml
```
Добавьте:
```
https://raw.githubusercontent.com/KronoZed/gentoo-overlay/master/repositories.xml
```
Должно получиться так:
```
overlays  : http://www.gentoo.org/proj/en/overlays/repositories.xml
https://raw.githubusercontent.com/KronoZed/gentoo-overlay/master/repositories.xml
```
После этого выполните:
```
layman -L
layman -a kronoz
```
#### Пакеты (стабильные)
* dev-python/aiodns (1.0.1)
* dev-python/pycares (1.0.0)
* dev-python/slixmpp (9999)
* games-fps/urbanterror-maps (20160214)
* games-util/urtconnector (9999)
* net-im/poezio (9999)
#### Пакеты (тестовые)
* games-util/urtdsc (9999)