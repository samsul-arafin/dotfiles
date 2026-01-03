# 🔧 Dotfiles
This is my personal configuration files. This repository contains my customized setup for a Hyprland environment on Linux.

# 📂 Directory Structure
```
.
├── .config
│   ├── hypr/           # Hyprland (WM, Idle, Lock)
│   ├── kitty/          # Terminal Emulator
│   ├── neofetch/       # System Info Tool
│   ├── rofi/           # Application Launcher & Menus
│   └── waybar/         # Status Bar
├── .local
│   └── bin/            # Custom Scripts (Rofi menus, etc.)
└── README.md
```

# 🛠 Prerequisites
Please ensure the following are installed on your system to make use of these configurations:
- **GNU Stow** (Recommended for installation)
- **Git**
- **Hyprland** (Window Manager)
  - **hypridle** (Idle daemon)
  - **hyprlock** (Screen locker)
- **Waybar** (Status bar)
- **Rofi** (Launcher)
  - **rofi-calc** (Calculator plugin)
- **Kitty** (Terminal)
- **Neofetch** (System info)

## Script Dependencies
These tools are required for the custom scripts in .local/bin:

- **NetworkManager** (**nmcli**) - Required for **rofi-wifimenu**
- **swww** - Wallpaper daemon (Required for **rofi-wallchanger**)
- **pywal** & **Matugen** - Color scheme generation
- **Gum** - Interactive shell prompts (Required for **webapp-install**)
- **scrcpy** - Android screen mirroring (Required for **sxp**)
- **Browser** - **Brave**, Chrome, Chromium, or Firefox (Required for **webapp-launch**)

## 📥 Installation Commands (Arch Linux)
These configurations are optimized for Arch Linux. You can install most dependencies using `pacman` and an AUR helper (like `yay`).
```
# 1. Official Repositories
sudo pacman -S git stow hyprland hypridle hyprlock waybar rofi rofi-calc kitty neofetch python-pywal scrcpy gum

# 2. AUR Packages (swww, matugen)
# You need an AUR helper like yay or paru
yay -S swww matugen-bin

```
_Note: For other distributions (Fedora, Debian, etc.), package names may differ, and you may need to build Hyprland tools from source.
_
# 🚀 Installation
1. **Clone the Repository:**
  Clone this repo to your home directory
    ```
     git clone [https://github.com/samsul-arafin/dotfiles.git](https://github.com/samsul-arafin/dotfiles.git) ~/.dotfiles
    cd ~/.dotfiles
    ```
2. **Apply Configurations:**
  I use GNU Stow to manage symlinks. This will link the contents of the `.config` and `.local` directories in this repository to your home folder.
  **To install everything:**
   ```bash
   stow .
   ```
# 📜 Custom Scripts


