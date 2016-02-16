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
paste_max_lines = 1
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
buddylist.color_bg = default
buddylist.color_delim = default
buddylist.color_fg = default
buddylist.conditions = ""
buddylist.filling_left_right = vertical
buddylist.filling_top_bottom = horizontal
buddylist.hidden = off
buddylist.items = "buddylist"
buddylist.position = bottom
buddylist.priority = 0
buddylist.separator = on
buddylist.size = 0
buddylist.size_max = 0
buddylist.type = root
buffers.color_bg = default
buffers.color_delim = default
buffers.color_fg = default
buffers.conditions = ""
buffers.filling_left_right = vertical
buffers.filling_top_bottom = columns_vertical
buffers.hidden = off
buffers.items = "buffers"
buffers.position = top
buffers.priority = 0
buffers.separator = on
buffers.size = 0
buffers.size_max = 0
buffers.type = root
input.color_bg = default
input.color_delim = cyan
input.color_fg = default
input.conditions = ""
input.filling_left_right = vertical
input.filling_top_bottom = horizontal
input.hidden = off
input.items = "[time],[buffer_plugin+.+buffer_short_name],[input_search],[input_paste],input_text+minimal"
input.position = bottom
input.priority = 1000
input.separator = off
input.size = 0
input.size_max = 5
input.type = window
isetbar.color_bg = default
isetbar.color_delim = cyan
isetbar.color_fg = default
isetbar.conditions = ""
isetbar.filling_left_right = vertical
isetbar.filling_top_bottom = horizontal
isetbar.hidden = on
isetbar.items = "isetbar_help"
isetbar.position = top
isetbar.priority = 0
isetbar.separator = on
isetbar.size = 3
isetbar.size_max = 3
isetbar.type = window
main_menu.color_bg = darkgray
main_menu.color_delim = lightblue
main_menu.color_fg = gray
main_menu.conditions = ""
main_menu.filling_left_right = vertical
main_menu.filling_top_bottom = horizontal
main_menu.hidden = on
main_menu.items = "*,main_menu"
main_menu.position = top
main_menu.priority = 10000
main_menu.separator = off
main_menu.size = 0
main_menu.size_max = 0
main_menu.type = root
menu_help.color_bg = gray
menu_help.color_delim = default
menu_help.color_fg = darkgray
menu_help.conditions = ""
menu_help.filling_left_right = vertical
menu_help.filling_top_bottom = horizontal
menu_help.hidden = on
menu_help.items = "menu_help"
menu_help.position = top
menu_help.priority = 9998
menu_help.separator = on
menu_help.size = 0
menu_help.size_max = 0
menu_help.type = root
nicklist.color_bg = default
nicklist.color_delim = cyan
nicklist.color_fg = default
nicklist.conditions = "${nicklist}"
nicklist.filling_left_right = vertical
nicklist.filling_top_bottom = columns_vertical
nicklist.hidden = on
nicklist.items = "buffer_nicklist"
nicklist.position = right
nicklist.priority = 200
nicklist.separator = on
nicklist.size = 0
nicklist.size_max = 0
nicklist.type = window
status.color_bg = red
status.color_delim = cyan
status.color_fg = default
status.conditions = ""
status.filling_left_right = vertical
status.filling_top_bottom = horizontal
status.hidden = on
status.items = "[time],[buffer_last_number],[buffer_plugin],buffer_number+:+buffer_name+(buffer_modes)+{buffer_nicklist_count}+buffer_zoom+buffer_filter,scroll,[lag],[hotlist],completion"
status.position = bottom
status.priority = 500
status.separator = off
status.size = 1
status.size_max = 0
status.type = window
sub_menu.color_bg = gray
sub_menu.color_delim = lightmagenta
sub_menu.color_fg = black
sub_menu.conditions = ""
sub_menu.filling_left_right = vertical
sub_menu.filling_top_bottom = columns_vertical
sub_menu.hidden = on
sub_menu.items = "*sub_menu"
sub_menu.position = top
sub_menu.priority = 9999
sub_menu.separator = on
sub_menu.size = 0
sub_menu.size_max = 0
sub_menu.type = root
title.color_bg = red
title.color_delim = cyan
title.color_fg = default
title.conditions = ""
title.filling_left_right = vertical
title.filling_top_bottom = horizontal
title.hidden = on
title.items = "buffer_title"
title.position = top
title.priority = 500
title.separator = off
title.size = 1
title.size_max = 0
title.type = window
urlbar.color_bg = default
urlbar.color_delim = default
urlbar.color_fg = default
urlbar.conditions = ""
urlbar.filling_left_right = vertical
urlbar.filling_top_bottom = horizontal
urlbar.hidden = off
urlbar.items = "urlbar_urls"
urlbar.position = bottom
urlbar.priority = 0
urlbar.separator = on
urlbar.size = 0
urlbar.size_max = 0
urlbar.type = root
window_popup_menu.color_bg = gray
window_popup_menu.color_delim = lightmagenta
window_popup_menu.color_fg = black
window_popup_menu.conditions = "active"
window_popup_menu.filling_left_right = vertical
window_popup_menu.filling_top_bottom = columns_vertical
window_popup_menu.hidden = on
window_popup_menu.items = "*window_popup_menu"
window_popup_menu.position = bottom
window_popup_menu.priority = 0
window_popup_menu.separator = on
window_popup_menu.size = 0
window_popup_menu.size_max = 0
window_popup_menu.type = window
```

#### [filter]

```
irc_smart = on;*;irc_smart_filter;*
```

