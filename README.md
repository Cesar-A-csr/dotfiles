# *WMs-config*

Config files for Sway a tiling Wayland compositor & Niri a scrollable tiling Wayland compositor.

### Why I Do This

Currently, as I write this, I am a relatively new user of the Free Open-Source world and GNU/Linux.
I started with Ubuntu 25.10 on a Desktop PC, then on a laptop from 2015-2016 with MX Linux.
Since then, I have learned and understood many things, and I wanted to try a Wayland Window Managers (WM) like:
- `Sway/SwayFX`
- `Niri`
- `MangoWC`
- More...

This is a personal project, and I hope if anyone reads this, it will be useful and give you new ideas, like me when I looked up for many things. Thanks.

## What's install?

|               Component               |                                       Purpose                                     |
| ------------------------------------- | --------------------------------------------------------------------------------- |
| `sway`                                | A tiling Wayland compositor                                                       |
| `swayidle`                            | Idle daemon                                                                       |
| `swaybg`                              | Wallpaper utility for Wayland compositor                                          |
| `waybar`                              | Customizable Wayland bar                                                          |
| `greetd`                              | Login manager daemon                                                              |
| `gtkgreeter`                          | GTK based greeter for greetd                                                      |
| `gtklock`                             | Lock screen                                                                       |
| `cage`                                | A Wayland kiosk compositor use to start gtkgreeter                                |
| `wezterm`/`foot`/`alacritty`          | Terminals (wezterm main, foot sway's default, alacritty niri's default)           |
| `thunar`                              | File manager                                                                      |
| `yazi`                                | TUI file manager                                                                  |
| `wofi`                                | Launcher / more function coming soon                                              |
| `nala`                                | Command line frontend for the APT package manager                                 |
| `nwg-displays`                        | Output management utility for Wayland compositors                                 |
| `nwg-look`                            | GTK3 settings editor for wlroots environments                                     |
| `baobab`                              | Disk usage analyzer                                                               |
| `gdu`/`ncdu`                          | TUI disk usage analyzer                                                           |
| `gparted`                             | Partition editor                                                                  |
| `lxpolkit`                            | PolicyKit authentication agent                                                    |
| `gammastep`                           | Set color temperature of display according to time of day                         |
| `pipewire`                            | Audio and video processing engine                                                 |
| `pavucontrol`                         | Based volume control tool                                                         |
| `helvum`                              | GTK patchbay for pipewire                                                         |
| `swappy`                              | A Wayland native snapshot and editor tool                                         |
| `cliphist` + `wl-clipboard`           | Clipboard history                                                                 |
| `grim` + `slurp`                      | Screenshot tools                                                                  |
| `gnome-text-editor`                   | Text editor                                                                       |
| `loupe`                               | Image viewer                                                                      |
| `mpv`                                 | Video player                                                                      |
| `brightnessctl`                       | Brightness controler                                                              |
| `tlp`                                 | Optimize laptop battery life                                                      |
| `xdg-desktop-portal/-wlr/-gtk`        | Wayland portals for sway                                                          |
| `nmtui`                               | TUI for controlling NetworkManager                                                |
| `bluetoothctl`                        | Bluetooth Control Command Line Tool (rarely used, there are better opt)           |

## Keybinding

|               Key Combo                               |                          Action                           |
|-------------------------------------------------------|-----------------------------------------------------------|
| `Super + t`                                           | Launch terminal                                           |
| `Super + q`                                           | Close focused window                                      |
| `Super + Space`                                       | App launcher                                              |
| `Super + e`                                           | Launch file manager                                       |
| `Super + x`                                           | Lock screen (gtklock)                                     |
| `Super + Shift + r`                                   | Reload Sway config                                        |
| `Super + Shift + w`                                   | Reload waybar                                             |
| `Super + Shift + q`                                   | Exit Sway                                                 |
| `Super + arrows`                                      | Move the focus in windows                                 |
| `Super + h/j/k/l`                                     | Move the focus in windows (vim style)                     |
| `Super + Shift + arrows`                              | Move the focus windows                                    |
| `Super + Shift + h/j/k/l`                             | Move the focus windows (vim style)                        |
| `Super + Ctrl + arrows`                               | Resize window                                             |
| `Super + Ctrl + h/j/k/l`                              | Resize window (vim style)                                 |
| `Super + 1-9/0`                                       | Switch to workspace 1-10                                  |
| `Super + Shift + 1-9/0`                               | Move focus windows to workspace 1-10                      |
| `Super + b`                                           | Split vertical                                            |
| `Super + v`                                           | Split horizontal                                          |
| `Super + w`                                           | Toggle split                                              |
| `Super + f`                                           | Fullscreen                                                |
| `Super + Shift + space`                               | Floating toggle                                           |
| `Super + Alt + space`                                 | Focus between the tiling window and the floating window   |
| `Super + minus`                                       | Move to scratchpad                                        |
| `Super + Shift + minus`                               | Scratchpad show                                           |
| `Print`                                               | Take full screenshot                                      |
| `Super + Print`                                       | Take screenshot of selected area                          |
| `Super + Shift + Print`                               | Take screenshot of focus window                           |
| `Ctrl + Print`                                        | Take full screenshot and copy to clipboard                |
| `Ctrl + Super + Print`                                | Take screenshot of selected area and copy to clipboard    |
| `Ctrl + Alt + Print`                                  | Take screenshot of focus window and copy to clipboard     |
| `Super + Shift + s`                                   | Open Swappy with the screenshot on the clipboard          |

## What's new

Hello there, this section is made to know what the most new feature add, done or modify in the dotfiles and in this repository ;]

### A new section

I made a new section called "**What's new**", there you will find the most recent work and modification I have done. It is posible you will find a whole explanation of why I did it, how I did it and more, it will depend on what is the new feature.

### The gtklock style and design

Gtklock is a lockscreen based in gtkgreet the look it basically the same, is familiar, I didn't want it to have really different looks and design between the greeter and the locker. I know there are some lighter or more customized options, such as swaylock, waylock, hyprlock, but in the end I decided on gtklock. \
Gtklock use a .ini file, a .css file, and also use .xml file to have a layout, this feature is pretty interesting, basically you can have your lockscreen the way you want. I use a layout.xml that is just the design of gnome lockscreen. Why? well I have use Gnome DE and I liked it, so this feature was perfect to me, at least to try it. \
The question now is: How did I do it? Luckily, someone had already done it and I found it when I was looking for a lockscreen, I copied the layout.xml and modified just a little. \
The repo is [https://github.com/tomdewildt/gnome-gtklock-theme/tree/master](https:/github.com/tomdewildt/gnome-gtklock-theme/tree/master) \
I used the layout and style, and modified them to my liking. I created four .css files: two with light styling and two with dark styling, two of them use corrupter, and the other two are "defaults". \
I will have to still do some 'features' specific with the default files, but that will be done later.

### gtklock + corrupter

What is corrupter? [https://github.com/r00tman/corrupter](https://github.com/r00tman/corrupter) \
corrupter is a **Simple image glitcher suitable for producing nice looking i3lock backgrounds.** \
It is written in Go and as the name suggests it glitchs the image, you provide a normal image (.png), then you have it glitched (.png). \
I use it with gtklock using a background image that is glitch by corrupter, I did this with a script called `corrupter-lockscreen`, but before all of that I had to do a few things. \
I had to install Go in my system. You can find many tutorial and also read Go documentation to do this. \
Then I cloned corrupter's repository and followed the "Getting Started" section, from there, I could use corrupter without any "problem", except for just a little detail, every time I wanted to use it, I had to specify the path to the binary file. To solve this "problem" I used symbolics link. \
`~$ ln -s ~/corrupter/corrupter ~/.local/bin/` \
After all, I could use corrupter without specifying the binary path, just by typing _corrupter_ in the terminal worked. Then I made the bash script `corrupter-lockscreen`. \
Basically what it does is:

1. It takes a screenshot with grim in .png and saves it to the `/tmp/` directory
2. Corrupter takes the screenshot and glitches the image
3. We convert the glitched pic to grayscale and analyze whether is mostly light or dark
4. Depending on the result mostly dark/light we use a specific .css file
5. finally we called gtklock with the chosen style and delete the two screenshots

## To do

- [x] Config gtklock and add some keybind to lock screen
- [x] Compile and use corrupter with gtklock
- [ ] Use swaync and config
- [ ] Check the gtk-modules (userinfo/powerbar/playerctl)
- [ ] Check some logout menus or add funcionality with wofi to use as a logout menu
- [ ] Make something to change background with wofi + swaybg and be more automatic 
- [ ] Make something to have a history with cliphist + wofi
- [x] Consider to add extra sections in the repo like 'What I learnt / Why I did this or use this / What's new' 


## Soon or Later

I have many things to add and do like improving and add the missings things in this repo, also in my systems I have a greeter and lock screen, but it doesn't have a style just default and more missings tools, but step-by-step I will keep going, *see you soon*.

### Thanks to
by now this is a secret ;]
