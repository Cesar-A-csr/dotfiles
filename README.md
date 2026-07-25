# *WMs-config*

Config files for Sway a tiling Wayland compositor & Niri a scrollable tiling Wayland compositor.

### Why I Do This

Currently, as I write this, I am a relatively new user of the Free Open-Source world and GNU/Linux.
I started with Ubuntu 25.10 on a Desktop PC, then on a laptop from 2015-2016 with MX Linux.
Since then, I have learned and understood many things, and I wanted to try a Wayland Window Managers (WM) like:
- `Sway`
- `Niri`
- `SwayFX`
- `MangoWC`
- More...

This is a personal project, and I hope if anyone reads this, it will be useful and give you new ideas, like me when I looked up for many things. Thanks.

## What's install?

| Component | Purpose |
| --------- |-------- |
| `sway` | A tiling Wayland compositor |
| `swayidle` | Idle daemon |
| `swaybg` | Wallpaper utility for Wayland compositor |
| `waybar` | Customizable Wayland bar |
| `greetd` | Login manager daemon |
| `gtkgreeter` | GTK based greeter for greetd |
| `gtklock` | Lock screen |
| `cage` | A Wayland kiosk compositor use to start gtkgreeter |
| `wezterm`, `foot`, `alacritty` | Terminals (wezterm main, foot lightweight/default in sway, alacritty default in niri) |
| `thunar` | File manager |
| `yazi` | TUI file manager |
| `wofi` | Launcher / more function coming soon |
| `nala` | Command line frontend for the APT package manager | 
| `nwg-displays` | Output management utility for Wayland compositors | 
| `nwg-look` | GTK3 settings editor for wlroots environments |
| `baobab` | Disk usage analyzer | 
| `gdu`, `ncdu` | TUI disk usage analyzer | 
| `gparted` | Partition editor |
| `lxpolkit` | PolicyKit authentication agent | 
| `gammastep` | Set color temperature of display according to time of day |
| `pipewire` | Audio and video processing engine |
| `pavucontrol` | Based volume control tool |
| `helvum` | GTK patchbay for pipewire |
| `swappy` | A Wayland native snapshot and editor tool |
| `cliphist` + `wl-clipboard` | Clipboard history |
| `grim` + `slurp` | Screenshot tools |
| `gnome-text-editor` | Text editor |
| `loupe` | Image viewer |
| `mpv` | Video player |
| `brightnessctl`  | Brightness controler |
| `tlp` | Optimize laptop battery life |
| `xdg-desktop-portal/-wlr/-gtk`| Wayland portals for sway |
| `nmtui` | TUI for controlling NetworkManager |
| `bluetoothctl` | Bluetooth Control Command Line Tool (rarely used, there are better opt) |

## Keybinding

| Key Combo | Action |
|-----------|--------|
| `Super + t` | Launch terminal |
| `Super + q` | Close focused window |
| `Super + Space` | App launcher |
| `Super + e` | Launch file manager |
| `Super + Shift + r` | Reload Sway config |
| `Super + Shift + w` | Reload waybar |
| `Super + Shift + q` | Exit Sway |
| `Super + h/j/k/l` or `Super + arrows` | Move the focus in windows |
| `Super + Shift + h/j/k/l` or `Super + Shift + arrows` | Move the focus windows |
| `Super + 1-9/0` | Switch to workspace 1-10 |
| `Super + Shift + 1-9/0` | Move focus windows to workspace 1-10 |
| `Super + b` | Split vertical |
| `Super + v` | Split horizontal |
| `Super + w` | Toggle split |
| `Super + f` | Fullscreen |
| `Super + Shift + space` | Floating toggle |
| `Super + a` | Focus all windows |
| `Super + Shift+minus` | move to scratchpad |
| `Super + minus` | scratchpad show |
| `Super + r` | "resize" mode |
| `Return` or `Escape` | On "resize" mode return to "default" mode |
| `Print` | Take full screenshot |
| `Super + Print` | Take screenshot of selected area |
| `Super + Shift + Print` | Take screenshot of focus window |
| `Ctrl + Print` | Take full screenshot and copy to clipboard |
| `Ctrl + Super + Print` | Take screenshot of selected area and copy to clipboard |
| `Ctrl + Alt + Print` | Take screenshot of focus window and copy to clipboard |
| `Super + Shift + s` | Open Swappy with the screenshot on the clipboard |

## To Do

- [ ] Config gtklock
- [x] Create a 30-outputs.conf.bak file as example
- [ ] Consider to compile and use corrupter with gtklock
- [ ] Check some logout menus or add funcionality with wofi to use as a logout menu
- [ ] Config something to change background with wofi + swaybg and be more automatic 
- [ ] Config something to have a history with cliphist + wofi
- [ ] Install some notification daemon
- [ ] Consider to add extra sections in the repo like 'What I learnt / Why I did this or use this / What's new' 

## Soon or Later

I have many things to add and do like improving and add the missings things in this repo, also in my systems I have a greeter and lock screen, but it doesn't have a style just default and more missings tools, but step-by-step I will keep going, **see you soon.**

### Thanks To
by now this is a secret ;]
