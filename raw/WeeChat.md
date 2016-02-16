title: WeeChat
category: Связанное с десктопом
---

#### weechat.conf

#### [look]

```
bare_display_time_format = "%H:%M:%S"
buffer_time_format = ""
highlight = "kron*,кроноз*,сударь"
item_time_format = "%H:%M:%S"
mouse = on
paste_max_lines = 5
prefix_same_nick = "\"
prefix_suffix = ""
save_config_on_exit = off
save_layout_on_exit = all
```

#### [color]

```
chat_highlight_bg = default
chat_nick_colors = "cyan,magenta,green,brown,lightblue,default,lightcyan,lightmagenta,lightgreen,blue,31,35,38,40,49,63,70,80,92,99,112,126,130,138,142,148,160,162,167,169,174,176,178,184,186,210,212,215,247"
```

#### [bar]

```
buddylist.items = "buddylist"
buffers.items = "buffers"
input.items = "[time],[buffer_plugin+.+buffer_short_name],[input_search],[input_paste],input_text+minimal"
isetbar.items = "isetbar_help"
main_menu.items = "*,main_menu"
menu_help.items = "menu_help"
sub_menu.items = "*sub_menu"
urlbar.items = "urlbar_urls"
window_popup_menu.items = "*window_popup_menu"
```

#### [filter]

```
irc_smart = on;*;irc_smart_filter;*
```

#### irc.conf

#### [look]

```
server_buffer = independent
```

#### [color]

```
nick_prefixes = "q:lightred;a:lightcyan;o:lightgreen;h:lightmagenta;v:yellow;*:lightblue"
```

#### [ctcp]

```
version = "I'm running WeeChat $version on $osinfo, it rocks!"
```