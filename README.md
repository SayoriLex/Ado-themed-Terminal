![<img width="945" height="485" alt="pasteds file" src="https://github.com/user-attachments/assets/a016019d-aa7d-4305-9381-4bc00739ad78" />]

# 🖤 Ado-themed-Terminal ▶️

A custom terminal color scheme inspired by **Ado**


# Prerequisites & Dependencies

Before setting up, make sure you have the following installed on your system:

-     Terminal: Kitty
-     Fetch Tool: Fastfetch
-     Font: Any Nerd Font (e.g., FiraCode Nerd Font)
-     Shell Tools: bash-completion, git, make

- sudo pacman -S kitty fastfetch bash-completion git make

![<img width="510" height="372" alt="pasted file" src="https://github.com/user-attachments/assets/bfd650d5-3db9-49da-8318-b4f2648d010f" />]

## Quick Installation

Simply clone this repository directly into your `~/.config` directory:

cd ~/.config
git clone [https://github.com/SayoriLex/Ado-themed-Terminal.git](https://github.com/SayoriLex/Ado-themed-Terminal.git)

####Predictive Bash (ble.sh)

To enable Fish-like autosuggestions directly in Bash:
Bash

## Clone and build ble.sh
git clone --recursive [https://github.com/akinomyoga/ble.sh.git](https://github.com/akinomyoga/ble.sh.git) ~/.local/share/blesh
cd ~/.local/share/blesh
make

Add the following lines at the end of your ~/.bashrc:
Bash

## bash-completion
if [ -f /usr/share/bash-completion/bash_completion ]; then
    . /usr/share/bash-completion/bash_completion
fi

## Auto-launch Fastfetch
if command -v fastfetch &> /dev/null; then
    fastfetch
fi

## Load ble.sh (Predictive Bash)
[[ $- == *i* ]] && source ~/.local/share/blesh/out/ble.sh


![<img width="1000" height="1000" alt="61kMyE7hKcL _SL1000_" src="https://github.com/user-attachments/assets/545e3634-8909-4356-92cc-2a12c9f20235" />]

### Colors Used

- background              #0B0E14
- foreground              #D5DCF0

- selection_background    #1D263B
- selection_foreground    #FFFFFF

- cursor                  #38BDF8
- cursor_text_color       #0B0E14
- 
### Normal Colors
- color0                  #151B26
- color1                  #E25B7B 
- color2                  #2DD4BF 
- color3                  #EAB308
- color4                  #38BDF8
- color5                  #A855F7
- color6                  #67E8F9
- color7                  #94A3B8
- 
### Bright Colors
- color8                  #475569 
- color9                  #FB7185
- color10                 #5EEAD4
- color11                 #FDE047
- color12                 #7DD3FC
- color13                 #C084FC
- color14                 #A5F3FC
- color15                 #F8FAFC

## ⚠️ Troubleshooting & Known Issues
If the album artwork isn't displaying correctly or appears stretched/broken in `fastfetch`:

- **Kitty Graphics Protocol (Recommended):** By default, this setup uses Kitty's native graphics protocol (`"type": "kitty or chafa"` in `config.jsonc`), which offers sharp, hardware-accelerated rendering without external dependencies.


🖤 Credits

    Color & aesthetics: Inspired by Ado (アド) the singer.

    Bash Engine: ble.sh.

    System Info: Fastfetch.
