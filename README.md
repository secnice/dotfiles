# Use the following code to your bashrc to get powerline after login, on a Debian box. Just install powerline from debian's official repo before!

export TERM="screen-256color"
powerline-daemon -q
POWERLINE_BASH_CONTINUATION=1
POWERLINE_BASH_SELECT=1
. /usr/share/powerline/bindings/bash/powerline.sh

# Command to save readonly files. :W saves file with sudo
command W w !sudo tee %


# Setting up powerline on vimrc config file
" Powerline settings
set laststatus=2 " Always display the status-line in all windows
set showtabline=2 " Always display the tabline even if there is only one tab
set t_Co=256 " Always display the status-line inside when inside tmux

