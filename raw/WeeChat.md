title: WeeChat
category: Связанное с десктопом
---

#### weechat.conf

[startup]

```
command_after_plugins = ""
command_before_plugins = ""
display_logo = on
display_version = on
sys_rlimit = ""
```

[look]

```
[look]
align_end_of_lines = message
bar_more_down = "++"
bar_more_left = "<<"
bar_more_right = ">>"
bar_more_up = "--"
bare_display_exit_on_input = on
bare_display_time_format = "%H:%M:%S"
buffer_auto_renumber = on
buffer_notify_default = all
buffer_position = end
buffer_search_case_sensitive = off
buffer_search_force_default = off
buffer_search_regex = off
buffer_search_where = prefix_message
buffer_time_format = ""
color_basic_force_bold = off
color_inactive_buffer = on
color_inactive_message = on
color_inactive_prefix = on
color_inactive_prefix_buffer = on
color_inactive_time = off
color_inactive_window = on
color_nick_offline = off
color_pairs_auto_reset = 5
color_real_white = off
command_chars = ""
command_incomplete = off
confirm_quit = off
confirm_upgrade = off
day_change = on
day_change_message_1date = "-- %a, %d %b %Y --"
day_change_message_2dates = "-- %%a, %%d %%b %%Y (%a, %d %b %Y) --"
eat_newline_glitch = off
emphasized_attributes = ""
highlight = "kron*,кроноз*,сударь"
highlight_regex = ""
highlight_tags = ""
hotlist_add_conditions = "${away} || ${buffer.num_displayed} == 0"
hotlist_buffer_separator = ", "
hotlist_count_max = 2
hotlist_count_min_msg = 2
hotlist_names_count = 3
hotlist_names_length = 0
hotlist_names_level = 12
hotlist_names_merged_buffers = off
hotlist_prefix = "H: "
hotlist_remove = merged
hotlist_short_names = on
hotlist_sort = group_time_asc
hotlist_suffix = ""
hotlist_unique_numbers = on
input_cursor_scroll = 20
input_share = none
input_share_overwrite = off
input_undo_max = 32
item_buffer_filter = "*"
item_buffer_zoom = "!"
item_mouse_status = "M"
item_time_format = "%H:%M:%S"
jump_current_to_previous_buffer = on
jump_previous_buffer_when_closing = on
jump_smart_back_to_buffer = on
key_bind_safe = on
key_grab_delay = 800
mouse = on
mouse_timer_delay = 100
nick_prefix = ""
nick_suffix = ""
paste_auto_add_newline = on
paste_bracketed = on
paste_bracketed_timer_delay = 10
paste_max_lines = 1
prefix_action = " *"
prefix_align = right
prefix_align_max = 0
prefix_align_min = 0
prefix_align_more = "+"
prefix_align_more_after = on
prefix_buffer_align = right
prefix_buffer_align_max = 0
prefix_buffer_align_more = "+"
prefix_buffer_align_more_after = on
prefix_error = "=!="
prefix_join = "-->"
prefix_network = "--"
prefix_quit = "<--"
prefix_same_nick = "\"
prefix_suffix = ""
quote_nick_prefix = "<"
quote_nick_suffix = ">"
quote_time_format = "%H:%M:%S"
read_marker = line
read_marker_always_show = off
read_marker_string = "- "
save_config_on_exit = off
save_layout_on_exit = all
scroll_amount = 3
scroll_bottom_after_switch = off
scroll_page_percent = 100
search_text_not_found_alert = on
separator_horizontal = "-"
separator_vertical = ""
tab_width = 1
time_format = "%a, %d %b %Y %T"
window_auto_zoom = off
window_separator_horizontal = on
window_separator_vertical = on
window_title = "WeeChat ${info:version}"
word_chars_highlight = "!\u00A0,-,_,|,alnum"
word_chars_input = "!\u00A0,-,_,|,alnum"
```

[color]

```
bar_more = lightmagenta
chat = default
chat_bg = default
chat_buffer = white
chat_channel = white
chat_day_change = cyan
chat_delimiters = green
chat_highlight = yellow
chat_highlight_bg = default
chat_host = cyan
chat_inactive_buffer = default
chat_inactive_window = default
chat_nick = lightcyan
chat_nick_colors = "cyan,magenta,green,brown,lightblue,default,lightcyan,lightmagenta,lightgreen,blue,31,35,38,40,49,63,70,80,92,99,112,126,130,138,142,148,160,162,167,169,174,176,178,184,186,210,212,215,247"
chat_nick_offline = default
chat_nick_offline_highlight = default
chat_nick_offline_highlight_bg = blue
chat_nick_other = cyan
chat_nick_prefix = green
chat_nick_self = white
chat_nick_suffix = green
chat_prefix_action = white
chat_prefix_buffer = brown
chat_prefix_buffer_inactive_buffer = default
chat_prefix_error = yellow
chat_prefix_join = lightgreen
chat_prefix_more = lightmagenta
chat_prefix_network = magenta
chat_prefix_quit = lightred
chat_prefix_suffix = green
chat_read_marker = magenta
chat_read_marker_bg = default
chat_server = brown
chat_tags = red
chat_text_found = yellow
chat_text_found_bg = lightmagenta
chat_time = default
chat_time_delimiters = brown
chat_value = cyan
chat_value_null = blue
emphasized = yellow
emphasized_bg = magenta
input_actions = lightgreen
input_text_not_found = red
nicklist_away = cyan
nicklist_group = green
separator = blue
status_count_highlight = magenta
status_count_msg = brown
status_count_other = default
status_count_private = green
status_data_highlight = lightmagenta
status_data_msg = yellow
status_data_other = default
status_data_private = lightgreen
status_filter = green
status_more = yellow
status_mouse = green
status_name = white
status_name_ssl = lightgreen
status_nicklist_count = default
status_number = yellow
status_time = default
```

[completion]

```
base_word_until_cursor = on
command_inline = on
default_template = "%(nicks)|%(irc_channels)"
nick_add_space = on
nick_completer = ":"
nick_first_only = off
nick_ignore_chars = "[]`_-^"
partial_completion_alert = on
partial_completion_command = off
partial_completion_command_arg = off
partial_completion_count = on
partial_completion_other = off
```

[history]

```
display_default = 5
max_buffer_lines_minutes = 0
max_buffer_lines_number = 4096
max_commands = 100
max_visited_buffers = 50
```

[network]

```
connection_timeout = 60
gnutls_ca_file = "/etc/ssl/certs/ca-certificates.crt"
gnutls_handshake_timeout = 30
proxy_curl = ""
```

[bar]

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

[filter]

```
irc_smart = on;*;irc_smart_filter;*
```

