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

git clone [https://github.com/YOUR_USERNAME/TerminalAdoTheme.git](https://github.com/YOUR_USERNAME/TerminalAdoTheme.git)
cd TerminalAdoTheme
./install.sh

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

🖤 Credits

    Color & aesthetics: Inspired by Ado (アド) the singer.

    Bash Engine: ble.sh.

    System Info: Fastfetch.
    EOF

5. Hacer commit en Git

cd "$REPO_DIR"
git add .
git commit -m "feat: complete repo with fastfetch config, avatar, install script, and updated README"