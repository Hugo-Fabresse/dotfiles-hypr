# dotfiles-hypr

Hyprland configuration.
Minimal, black, rational.

---

## Stack

- **WM** : Hyprland
- **Lock** : Hyprlock
- **Background** : Swaybg (black)
- **Notifications** : Dunst
- **Widgets** : Calendar, Volume Input, Notification Panel (PyQt6)
- **Spotify PiP** : [Ash](https://github.com/Hugo-Fabresse/ash) (C++/Qt6)

---

## Dependencies

```bash
sudo pacman -S hyprland hyprlock swaybg dunst python python-pyqt6 python-requests python-dbus
yay -S maplemono-otf
```

---

## Install

```bash
git clone git@github.com:Hugo-Fabresse/dotfiles-hypr.git ~/dotfiles/hypr
ln -s ~/dotfiles/hypr ~/.config/hypr
```

Widget and shell scripts live in `~/dotfiles/scripts/` (see main dotfiles README for install steps).

---

## Keybinds

| Key | Action |
|-----|--------|
| Super + Return | Terminal |
| Super + n | Browser |
| Super + s | Spotify (spotify_player in Kitty) |
| Super + Shift + s | Ash (Spotify PiP toggle) |
| Super + d | Launcher |
| Super + v | Volume input |
| Super + p | Notification panel |
| Super + Shift + p | Clear notification history |
| Super + c | Clipboard history |
| Super + Shift + c | Wipe clipboard |
| Super + q | Close window |
| Super + Shift + q | Exit Hyprland |
| Super + f | Toggle float |
| Super + Space | Fullscreen |
| Super + b | Toggle Waybar |
| Super + m | Minimize |
| Super + Shift + m | Restore minimized |
| Super + Ctrl + l | Lock screen |
| Super + h/j/k/l | Move focus |
| Super + Shift + arrows | Resize window |
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
└── startup_bg.sh
```
