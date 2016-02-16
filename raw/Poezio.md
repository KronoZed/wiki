title: Poezio
category: Связанное с десктопом
---

#### poezio.cfg

```
[Poezio]

jid =
password =
default_nick =
rooms =
highlight_on =
plugins_autoload = admin:uptime:simple_notify:status:ping:day_change:time_marker
resource = poezio
server = anon.jeproteste.info
certificate =
ciphers = HIGH+kEDH:HIGH+kEECDH:HIGH:!PSK:!SRP:!3DES:!aNULL
ignore_certificate = true
force_encryption = true
whitespace_interval = 300
ca_cert_path =
auto_reconnect = true
connection_check_interval = 60
connection_timeout_delay = 10
send_initial_presence = true
status =
status_message =
save_status = true
custom_host =
custom_port =
use_bookmarks_method =
use_remote_bookmarks = true
after_completion = ,
add_space_after_completion = true
max_nick_length = 25
show_timestamps = true
words =
enable_xhtml_im = true
hide_exit_join = 120
hide_status_change = 120
information_buffer_popup_on = error roster warning help info
popup_time = 4
hide_user_list = true
filter_info_messages =
autorejoin = true
autorejoin_delay = 5
alternative_nickname =
muc_history_length = 50
use_log = true
load_log = 50
log_dir =
log_errors = true
plugins_dir =
plugins_conf_dir =
show_inactive_tabs = true
show_tab_names = true
show_tab_numbers = false
use_tab_nicks = true
show_muc_jid = false
show_roster_jids = false
show_s2s_errors = true
roster_show_offline = false
roster_sort = online:jid:show
roster_group_sort = name
beep_on = highlight private invite
themes_dir =
theme = dark
create_gaps = true
enable_vertical_tab_list = false
vertical_tab_list_size = 13
vertical_tab_list_sort = desc
user_list_sort = desc
display_user_color_in_join_part = false
display_tune_notifications = false
enable_carbons = false
enable_user_tune = true
display_gaming_notifications = false
enable_user_gaming = true
display_mood_notifications = false
enable_user_mood = true
display_activity_notifications = false
enable_user_activity = true
enable_user_nick = true
send_chat_states = true
send_poezio_info = true
send_os_info = false
send_time = false
separate_history = false
lang = ru
max_messages_in_memory = 4096
max_lines_in_memory = 4096
show_useless_separator = false
exec_remote = false
remote_fifo_path =
lazy_resize = true
show_jid_in_conversations = true
deterministic_nick_colors = true

[bindings]

M-i = ^I

[var]

folded_roster_groups =
info_win_height = 4

[simple_notify]

command = notify-send "New message from %(from)s" "%(body)s"

[time_marker]

delay = 600
```