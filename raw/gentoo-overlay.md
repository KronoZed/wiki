title: gentoo-overlay
category: Мои проекты
---

#### Установка

Вариант 1:

Выполните:

```
layman -f -o https://raw.githubusercontent.com/KronoZed/gentoo-overlay/master/repositories.xml -a kronoz
```

Вариант 2:

Чтобы добавить его в список layman`a, откройте **/etc/layman/layman.cfg** и сразу после строки:

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

* app-antivirus/clamtk (5.20) - A frontend for ClamAV using Gtk2-perl
* app-editors/atom-bin (1.5.4) - A hackable text editor for the 21st Century. - Binary package
* app-office/litetran (9999) - Very simple GUI for text translation (like google translate)
* dev-python/aiodns (1.0.1) - Simple DNS resolver for asyncio
* dev-python/pycares (1.0.0) - Python interface for c-ares
* dev-python/slixmpp (9999) - Python library for XMPP (branched from sleekxmpp)
* games-fps/urbanterror-maps (20160214) - various maps for urban terror 4
* games-util/urtconnector (9999) - Advanced UrbanTerror launcher program
* net-im/poezio (9999) - Console XMPP client that looks like most famous IRC clients
* x11-misc/twmn (9999) - A notification system for tiling window managers

#### Пакеты (тестовые)

* games-util/urtdsc (9999)
