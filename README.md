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
- GNU Stow (Recommended for installation)
- Git
- Hyprland (Window Manager)
  - hypridle (Idle daemon)
  - hyprlock (Screen locker)
- Waybar (Status bar)
- Rofi (Launcher)
  - rofi-calc (Calculator plugin)
- Kitty (Terminal)
- Neofetch (System info)

## Script Dependencies
These tools are required for the custom scripts in .local/bin:

- NetworkManager (nmcli) - Required for rofi-wifimenu
- swww - Wallpaper daemon (Required for rofi-wallchanger)
- pywal & Matugen - Color scheme generation
- Gum - Interactive shell prompts (Required for webapp-install)
- scrcpy - Android screen mirroring (Required for sxp)
- Browser - Brave, Chrome, Chromium, or Firefox (Required for webapp-launch)
