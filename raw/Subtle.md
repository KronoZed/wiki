title: Subtle
category: Связанное с десктопом
---
### Subtle - статический фреймовый оконный менеджер.

##### Эти элементы доступны для панелей:
```
:views     - Отобразит список тегов
:title     - Ответственен за включение/выключение названия текущего окна
:tray      - Показывать ли трей приложений
:keychain  - Display current chain (Can be used only once)
:sublets   - Отобразить все имеющиеся саблеты
:sublet    - Отобразить только некоторый саблет, требуется указать их имена
:spacer    - Влияет на местоположение элемента
:center    - Центрирует элемент панели
:separator - Показывать разделитель между элементами
icon       - Показывать иконку между элементами
```

##### Готовый пример панели:
```
screen 1 do
  top     [ :views, :separator, :title, :spacer, :tray, :seperator, :clock2 ]
end
```

##### Эти свойства доступны для большинства стилей:
```
foreground - Цвет текста переднего плана
background - Фоновый цвет
font       - Шрифт строки (xftontsel или xft)
margin     - Внешнее расстояние
border     - Цвет и размер границы
padding    - Внутренний интервал
active     - Цвет активного клиента
icon       - Цвет иконки
inactive   - Цвет неактивного клиента
panel      - Цвет панели
separator  - Цвет сепаратора
stripple   - This property sets the color of the panel stippling if any
width      - Это свойство определяет длину строки в символе, по умолчанию 50 символов
min_width  - Это свойство устанавливает минимальную ширину пикселя элемента панели
```

##### Кнопки мыши
```
B1 = Button1 (Левая кнопка мыши)
B2 = Button2 (Средняя кнопка мыши)
B3 = Button3 (Правая кнопка мыши)
B4 = Button4 (Колесо мыши вверх)
B5 = Button5 (Колесо мыши вниз)
```

##### Специальные клавиши-модификаторы:
```
[*A*] = левый Alt (Mod1)
[*C*] = Control клавиша
[*M*] = Meta клавиша (Mod3)
[*S*] = Shift клавиша
[*W*] = Super/Windows клавиша (Mod4)
[*G*] = AltGr клавиша (Mod5)
```

##### Общие клавиши
```
Space
Tab
Enter / Return
F1 - F12
Left, Down, Up, Right
Next, Prior
Page_Up, Page_Down
Home, End
Insert, Delete
Add, Subtract, Multiply, Divide, Equal
Decimal
Num_Lock
Escape
```

##### Мультимедийные клавиши
```
XF86AudioMute
XF86AudioRaiseVolume
XF86AudioLowerVolume
XF86AudioPlay
XF86AudioPrev
XF86AudioNext
XF86WWW
XF86Calculator
XF86Mail
```

##### Геометрия окон
```
X      - для размещения в направлении X
Y      - для размещения в направлении Y
WIDTH  - по ширине окна
HEIGHT - по высоте окна
:horz  - для горизонтального тайлинга
:vert  - для вертикального тайлинга
```

##### Примеры геометрии
```
gravity :c_a1,      [  33,  33,  34,  34 ]
gravity :c_a2,      [  25,  25,  50,  50 ], :vert
gravity :c_a3,      [   0,   0, 100, 100 ]

gravity :c_b1,      [   0,  33, 100,  34 ]
gravity :c_b2,      [  33,   0,  34, 100 ], :horz
```

##### Пример захвата гравитаций
```
grab "W-KP_5",      [ :c_a1,  :c_a2,  :c_a3,  :c_b1,  :c_b2         ]
```

##### Маркировка метками
```
Borderless - Это свойство позволяет безграничный режим для маркированных клиентов
Center     - Это свойство позволяет центрированный режим для маркированных клиентов
Fixed      - Это свойство позволяет фиксированный режим для маркированных клиентов
Float      - Это свойство позволяет свободный режим для маркированных клиентов
Full       - Это свойство позволяет полный экран для маркированных клиентов
Geometry   -
Gravity    - Это свойство задает определенную гравитацию к маркированому клиенту, но только на соответствующих рабочих столов
Match      - Это свойство добавляет matcher к тегу
on_match   -
position   -
resize     -
stick      -
type       -
urgent     -
zaphod     -
```

##### Типы определения приложений
```
:name     - Сопоставление имени окна
:instance - Сопоставление имени инстанции окна
:class    - Сопоставление имени класса окна
:role     - Сопоставление роли окна
:type     - Сопоставление типа окна
```

##### This property sets the tagged client to be treated as a specific window type though as the window sets the type itself
```
:normal  - Treat as normal window
:desktop - Treat as desktop window
:dock    - Treat as dock window
:toolbar - Treat as toolbar windows
:splash  - Treat as splash window
:dialog  - Treat as dialog window
```

##### Рабочие столы
```
match     -
gravity   -
icon      -
icon_only -
dynamic   -
```

##### Пример автоматического старта приложения
```
on :start do
  Subtlext::Client.spawn "app"
end
```
