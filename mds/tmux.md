#### WINDOWS
|||
|-|-|
`Ctrl + b &`|Close current window.
`Ctrl + b n`|Next window.
`Ctrl + b p`|Previous window.
`Ctrl + b 0...9`|Select window by number.
`Ctrl + b w`|List all windows.
`tmux new -s mysession -n mywindow`|start a new session with the name mysession and window mywindow.
`Ctrl + b c`|Create window.
`Ctrl + b ,`|Rename current window.
#### PANES
|||
|-|-|
`Ctrl +b [spacebar]`|Toggle between pane layouts.
`Ctrl + b !`|Convert pane into a window.
`Ctrl + b "`|Split pane horizontally.
`Ctrl + b {`|Move the current pane left.
`Ctrl + b x`|Close pane.
`: setw synchronize-panes`|(Command Mode) Toggle synchronize-panes(send command to all panes).
`Ctrl + b %`|Split pane vertically.
`Ctrl + b + [keyboard arrows]`|Resize current pane.
`Ctrl + b [keyboard arrows]`|Switch to pane to the direction.
`Ctrl + b ;`|Toggle last active pane.
`Ctrl + b }`|Move the current pane right.
`Ctrl + b z`|Toggle pane zoom.
`Ctrl + b q`|Show pane numbers(type the number to goto that pane).
`Ctrl + b o`|Switch to next pane.
#### MISC
|||
|-|-|
`Ctrl +b :`|Enter command mode.
`: setw -g OPTION`|(Command Mode) Set OPTION for all windows.
`: set -g OPTION`|(Command Mode) Set OPTION for all sessions.
`$ tmux ls | cut -d: -f1 | xargs -l1 tmux kill-session -t`|(Bash Mode) Kill all the tmux sessions.
#### COMMANDS
|||
|-|-|
`: set -g mouse-select-window on`|(Command Mode) Enable mouse select windows.
`: set -g status-justify centre`|(Command Mode) Center the window list.
`: setw -g monitor-activity on`|(Command Mode) Enable activity alerts.
`: setw -g mode-keys vi`|(Command Mode) Use vi keys in buffer.
`: set -g mouse-select-pane on`|(Command Mode) Enable mouse select panes.
`: set -g mouse-resize-pane on`|(Command Mode) Enable mouse resize panes.
`: set -g mode-mouse on`|(Command Mode) Enable mouse.
`: set -g visual-activity on`|(Command Mode) Enable activity alerts.
`: set -g default-terminal "screen-256color"`|(Command Mode) Set the default terminal mode to 256color mode.
#### HELP
|||
|-|-|
`$ tmux info`|(Bash Mode) Show every session, window, pane, etc..
`Ctrl +b ?`|Show shortcuts.
#### COPY MODE
|||
|-|-|
`Ctrl +b ]`|Paste contents of buffer_0.
`q`|Quit mode.
`[spacebar]`|Start selection.
`[enter]`|Copy selection.
`: show-buffer`|(Command Mode) Display buffer_0 contents.
`: capture-pane`|(Command Mode) Copy entire visible contents of pane to a buffer.
`: list-buffers`|(Command Mode) Show all buffers.
`: choose-buffer`|(Command Mode) Show all buffers and paste selected.
`Ctrl + b [`|Enter copy mode.
`: save-buffer buf.txt`|(Command Mode) Save buffer contents to buf.txt
`: delete-buffer -b 1`|(Command Mode) Delete buffer_1.
#### SESSIONS
|||
|-|-|
`Ctrl + b $`|Rename session.
`tmux new -s mysession`|Start a new session with the name mysession.
`tmux attach -d`|Enter last session and reset window size.
`tmux at`|Log in to the last session.
`Ctrl + b (`|Move to previous session.
`Ctrl + b d`|Detach from session.
`tmux kill-ses -t mysession`|Kill session mysession.
`Ctrl + b s`|Show all sessions.
`tmux a -t mysession`|Enter a session named mysession.
`tmux ls`|List all sessions.
`Ctrl + b )`|Move to the next session.
