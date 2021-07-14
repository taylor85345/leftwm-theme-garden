# Garden

## Packages

```
DE          : Arch
WM          : Leftwm
terminal    : Alacritty
bar         : Polybar
launcher    : Rofi
```

## Screenshot

![Desktop](./images/desktop1.png)
![Desktop](./images/tile.png)
![Desktop](./images/app_menu.png)
![Desktop](./images/dolphin.png)

## Dependencies

- [leftwm-git](https://github.com/leftwm/leftwm)
- [jonaburg picom](https://github.com/jonaburg/picom)
- [polybar](https://github.com/polybar/polybar)
- [inter nerd font](https://github.com/rsms/inter)
- [rofi](https://github.com/davatorium/rofi)

## Installation

1. Install all required dependencies

2. Clone the repository

```BASH
git clone https://github.com/taylor85345/leftwm-theme-garden.git
```

3. Make a copy of this project in your themes folder

```BASH
cp -r ./leftwm-theme-dracula-rounded ~/.config/leftwm/themes
```

4. Remove the symlink to your current theme if set

```BASH
rm ~/.config/leftwm/themes/current
```
5. Set this as your current theme

```BASH
ln -s ~/.config/leftwm/themes/leftwm-theme-garden ~/.config/leftwm/themes/current
```

6. Restart your window manager

```Default shortcut
$MOD + Shift + r
```

## Configuration

Coming Soon!

## Credits

This theme is heavily based on the Linear theme for AwesomeWM by manilarome(https://github.com/manilarome/the-glorious-dotfiles), and I have borrowed several configs and scripts from that theme. The base LeftWM configs were modified from the Dracula Rounded theme by AethanFoot (https://github.com/AethanFoot/leftwm-theme-dracula-rounded). I've still got some mismatched Dracula configs hanging around, and I'll be removing/updating those in the near future.
