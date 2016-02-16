title: URxvt
category: Desktop Related
---
#### My Configuration

```
! включить расширения на perl: основные, парсер регулярных выражений (для подсветки URL)
URxvt.perl-ext-common: default,matcher

! браузер для открытия ссылок
URxvt.url-launcher: /usr/bin/chromium

URxvt.matcher.button: 2
URxvt.colorUL: #cacc46
URxvt.underlineURLs: true
URxvt.underlineColor: #cacc46

! используемый шрифт
URxvt.font: xft:Droid sans mono Slashed:pixelsize=22
URxvt.boldFont: xft:Droid Sans Mono Slashed:bold

URxvt.saveLines: 5000

! геометрия (позиция, размер) окна (в символах). Стандартный размер: 80x24, увеличено для использования табов
URxvt.geometry: 100x35

URxvt.termName: rxvt-unicode-256color

! Псевдопрозрачность
URxvt.transparent: true

! уменьшение (-100 .. -1) или увеличение (0 .. 100) яркости прозрачного фона
URxvt.shading: 10

! скроллбар
URxvt.scrollBar: false

! стиль скроллбара
URxvt.scrollstyle: plain

! расположение скроллбара 
URxvt.scrollBar_right: true

! цвет скроллера
URxvt.scrollColor: #1A1A1A

URxvt.internalBorder: 10

! color the man
URxvt.colorMode: on
URxvt.boldColors: on
URxvt.dynamicColors: on
URxvt.colorULMode: on
URxvt.underLine: off
URxvt.colorBDMode: on
URxvt.colorBD:  cyan

! цвет фона
URxvt.background: #2c2c2c

! цвет переднего плана
URxvt.foreground: #dcdccc

URxvt.color0: #2c2c2c
URxvt.color1: #705050
URxvt.color2: #60b48a
URxvt.color3: #dfaf8f
URxvt.color4: #9ab8d7
URxvt.color5: #dc8cc3
URxvt.color6: #8cd0d3
URxvt.color7: #dcdccc
URxvt.color8: #709080
URxvt.color9: #dca3a3
URxvt.color10: #72d5a3
URxvt.color11: #f0dfaf
URxvt.color12: #94bff3
URxvt.color13: #ec93d3
URxvt.color14: #93e0e3
URxvt.color15: #ffffff

URxvt.tabbed.tabbar-fg: 2
URxvt.tabbed.tabbar-bg: 0
URxvt.tabbed.tab-fg: 3
URxvt.tabbed.tab-bg: 0
```