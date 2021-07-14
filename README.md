# Garden

## Packages

```
DE          : Manjaro
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
- [picom-jonaburg-git](https://github.com/jonaburg/picom)
- [polybar](https://github.com/polybar/polybar)
- [nerd-fonts-inter](https://github.com/rsms/inter)
- [rofi](https://github.com/davatorium/rofi)

## Installation

1. Install all required dependencies

2. cd into your Themes directory

```BASH
cd $HOME/.config/leftwm/themes
```

3. Clone the repository

```BASH
git clone https://github.com/taylor85345/leftwm-theme-garden.git Garden
```

4. Remove the symlink to your current theme if set

```BASH
rm current
```
5. Set this as your current theme

```BASH
ln -s Garden current
```

6. Restart your window manager

```Default shortcut
$MOD + Shift + r
```

## Configuration
  + **Default Apps script**
    
    I've included the default_app script (assigned to the '+' in polybar) which assigns a program to each tag and opens whichever application is assigned to the currently focused tag. You can edit the script, or you can copy `misc/default_apps.sh` to `$HOME/.config/leftwm` and edit that file if you want your selections to survive leftwm-theme updates.
  
    By default, the script will launch the following

    ```BASH
    TERM=alacritty
    BROWSER=firefox
    DOC=libreoffice
    FILE=dolphin
    PLAYER=vlc
    GAME=steam
    PHOTO=gimp
    SANDBOX=virtualbox
    DEV="alacritty -e vim";
    ```

  + **Application Theming**
    
    For consistency, I use the following themes in GTK and QT apps:
    
    - QT5/Kvantum: [Inverse-dark](https://github.com/yeyushengfan258/Inverse-dark-kde)
    - GTK: [gtk-theme-breath](https://github.com/manjaro/artwork-breath-gtk)

    I highly recommend using QT5 applications with this theme, particularly those made for the KDE desktop environment, and applying the Inverse-dark theme via `qt5ct` and `kvantum-manager`.
  
  + **Fetch Script**
    
    If for some reason you want to use my fetch script, you will need to install [Macchina](https://github.com/Macchina-CLI/macchina) and add the following to your .bashrc:

    ```BASH
    macchina -UbpS --custom-ascii ~/.config/leftwm/themes/current/misc/leaf.ascii --color blue --custom-ascii-color green
    ```

## Credits

This theme is heavily based on the Linear theme for AwesomeWM by manilarome(https://github.com/manilarome/the-glorious-dotfiles), and I have borrowed several configs and scripts from that theme. The base LeftWM configs were modified from the Dracula Rounded theme by AethanFoot (https://github.com/AethanFoot/leftwm-theme-dracula-rounded). I've still got some mismatched Dracula configs hanging around, and I'll be removing/updating those in the near future.
