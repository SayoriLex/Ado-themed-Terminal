# Prerequisites & Dependencies

Before setting up, make sure you have the following installed on your system:

-     Terminal: Kitty
-     Fetch Tool: Fastfetch
-     Font: Any Nerd Font (e.g., FiraCode Nerd Font)
-     Shell Tools: bash-completion, git, make

# On Arch Linux / EndeavourOS:
Bash

sudo pacman -S kitty fastfetch bash-completion git make

# Quick Setup
1. Auto Installation (Configs only)

Clone this repository and run the setup script:
Bash

git clone

2. Predictive Bash (ble.sh)

To enable Fish-like autosuggestions directly in Bash:
Bash

# Clone and build ble.sh
git clone --recursive [https://github.com/akinomyoga/ble.sh.git](https://github.com/akinomyoga/ble.sh.git) ~/.local/share/blesh
cd ~/.local/share/blesh
make

Add the following lines at the end of your ~/.bashrc:
Bash

# bash-completion
if [ -f /usr/share/bash-completion/bash_completion ]; then
    . /usr/share/bash-completion/bash_completion
fi

# Auto-launch Fastfetch
if command -v fastfetch &> /dev/null; then
    fastfetch
fi

# Load ble.sh (Predictive Bash)
[[ $- == *i* ]] && source ~/.local/share/blesh/out/ble.sh


# =================================
# Colors Used
# =================================
background              #0B0E14
foreground              #D5DCF0

selection_background    #1D263B
selection_foreground    #FFFFFF

cursor                  #38BDF8
cursor_text_color       #0B0E14

color0                  #151B26
color1                  #E25B7B 
color2                  #2DD4BF 
color3                  #EAB308
color4                  #38BDF8
color5                  #A855F7
color6                  #67E8F9
color7                  #94A3B8

color8                  #475569 
color9                  #FB7185
color10                 #5EEAD4
color11                 #FDE047
color12                 #7DD3FC
color13                 #C084FC
color14                 #A5F3FC
color15                 #F8FAFC

🖤 Credits

    Color & aesthetics: Inspired by Ado (アド) the singer.

    Bash Engine: ble.sh.

    System Info: Fastfetch.
