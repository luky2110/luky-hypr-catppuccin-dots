# Luky's Catppuccin Hyprland Dots
If you do not like something, change it youself but feel free to use it tho!

# Program preferences

File Explorer: Thunar (Super + E)

Terminal: Alacritty (Super + Enter)

Browser: Librewolf (Super + B)

App Launcher/Menu: Wofi (Super + Space)

Screenshooter: Grimblast (Super + S/PRT SC)

Archive Manager/Extractor: Engrampa

Media Player: VLC

Image Viewer: Loupe

Network: iwd + dhcpcd 

If you wish to use the programs that I prefer then copy and paste this
```
sudo pacman -S thunar iwd dhcpcd grimblast wofi librewolf alacritty thunar thunar-volman gvfs udisks2 vlc engrampa loupe
```

If you prefer to change the primary apps you will have to go into the config and change variables

# Recommended Programs
Without these your hyprland might not work as expected or miss features so please install all of these
```
sudo pacman -S waybar hyprpaper hyprshutdown playerctl qt5ct qt6ct qt5-wayland qt6-wayland ttf-jetbrains-mono-nerd polkit hyprpolkitagent xdg-desktop-portal-hyprland xdg-desktop-portal
```
After installation please also run this to enable them on boot
```
sudo systemctl enable --now polkit hyprpolkitagent
```

# Disclaimer
If you use a different terminal emulator than alacritty the shutdown button on the waybar might not work as it should.
The files you need to worry about if that is the case are

~/.config/waybar/power.sh

~/.config/hypr/hyprland.lua (In the window rule section)
