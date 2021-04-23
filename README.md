### Comfortable tmux

'''bash
unbind C-b
set-option -g prefix C-a
bind-key C-a send-prefix

set -g history-limit 10000
set -g allow-rename off

set-window-option -g mode-keys vi

bind b setw synchronize-panes
bind r source-file ~/.tmux.conf \; display-message "Config reloaded..."
'''
