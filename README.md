# Jacob's Build of the dmenu by [suckless](https://tools.suckless.org/dmenu/)

## Patches

- [Highlight](https://tools.suckless.org/dmenu/patches/highlight/)

- [Mouse support](https://tools.suckless.org/dmenu/patches/mouse-support/)

- [Numbers](https://tools.suckless.org/dmenu/patches/numbers/)

- [Xresources](https://tools.suckless.org/dmenu/patches/xresources/)

## Installation

```shell
git clone https://gitlab.com/Jacob_McDonnell/dmenu.git
cd dmenu
sudo make install
```

Users of Arch-based distros can install from the AUR, [dmenu-jacob-git](https://aur.archlinux.org/packages/dmenu-jacob-git/).

## Dependencies

- `pywal` for a dynamic color scheme

- [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra/)

## How to configure with Xresources

Many variables can be configured through `~/.Xdefaults` or `~/Xresources` but you must run `xrdb` on the file before the settings load.

For example fonts, transparency, or colors:

```
dmenu.font : IBM Plex Mono
dmenu.background : yellow
dmenu.foreground : green
dmenu.selbackground : blue
dmenu.selforeground : red
```

### Colors and Fonts

- Compatible with `pywal` for a dynamic color scheme

## Emojis

dmenu like many suckless programs will crash at the first sign of an emoji. The solution to install [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra/)
