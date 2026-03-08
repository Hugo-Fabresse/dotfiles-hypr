# dotfiles-hypr

Hyprland configuration.
Minimal, black, rational.

---

## Stack

- **WM** : Hyprland
- **Lock** : Hyprlock
- **Background** : Swaybg (black)
- **Notifications** : Mako
- **Widgets** : Calendar, Spotify PiP, Volume Input (PyQt6)

---

## Dependencies

```bash
sudo pacman -S hyprland hyprlock swaybg mako python python-pyqt6 python-requests python-dbus
yay -S maplemono-otf
```

---

## Install

```bash
git clone git@github.com:Hugo-Fabresse/dotfiles-hypr.git ~/dotfiles/hypr
ln -s ~/dotfiles/hypr ~/.config/hypr

# Copy widget scripts
mkdir -p ~/.local/bin
cp ~/dotfiles/hypr/bin/* ~/.local/bin/
chmod +x ~/.local/bin/*.py

# Copy shell scripts
mkdir -p ~/.local/share/hypr
cp ~/dotfiles/hypr/toggle_waybar.sh ~/.local/share/hypr/
cp ~/dotfiles/hypr/wofi_toggle.sh ~/.local/share/hypr/
chmod +x ~/.local/share/hypr/*.sh
```

---

## Keybinds

| Key | Action |
|-----|--------|
| Super + Return | Terminal |
| Super + n | Browser |
| Super + s | Spotify |
| Super + Shift + s | Spotify PiP |
| Super + d | Launcher |
| Super + v | Volume input |
| Super + q | Close window |
| Super + f | Toggle float |
| Super + Space | Fullscreen |
| Super + b | Toggle Waybar |
| Super + Ctrl + l | Lock screen |
| Super + h/j/k/l | Move focus |
| Super + Shift + h/j/k/l | Move window |
| Super + 1-0 | Switch workspace |
| Super + Shift + 1-0 | Move to workspace |
| Print | Screenshot |
| Shift + Print | Screenshot selection |

---

## Content

```
hypr/
├── hyprland.conf
├── hyprlock.conf
├── startup_bg.sh
├── toggle_waybar.sh
├── wofi_toggle.sh
└── bin/
    ├── my_calendar.py
    ├── spotify-pip.py
    └── volume_input.py
```
