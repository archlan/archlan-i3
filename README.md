# ArchLan Linux i3 skel

<p align="center">
<a href="https://archlan.github.io"><img src="https://raw.githubusercontent.com/archlan/assets/main/img/logo/128x128_logo.svg" height="128" width="128" alt="ArchLan"></a>
</p>


<p align="center">
  <img src="https://img.shields.io/badge/Released%3F-No-pink?style=flat-circle">
  <img src="https://img.shields.io/github/downloads/archlan/releases/total?style=social">
  <img src="https://img.shields.io/github/stars/archlan/iso?style=flat-circle&color=pink">
  <img src="https://img.shields.io/github/issues/archlan/iso?color=purple&style=flat-circle">
</p>

<p align="center">
<a href="https://www.archlinux.org">Arch</a> based distribution. Designed for fun and minimalism.
</p>

## Standalone setup for this configuration

1. [Prerequisites](#requirements)
2. [Install](#installation)
3. [Keybindings](#keybinds)

## Requirements
> This configuration needs some software to be installed before it is used;

**List of dependencies**
* [alacritty](https://github.com/alacritty/alacritty)
* [flameshot](https://github.com/flameshot-org/flameshot)
* [i3-gaps](https://github.com/Airblader/i3)
* [i3lock-color](https://github.com/Raymo111/i3lock-color)
* [picom-ibhagwan](https://github.com/ibhagwan/picom)
* [polybar](https://github.com/polybar/polybar)
* [pywal](https://github.com/dylanaraps/pywal)
* [rofi](https://github.com/davatorium/rofi)
* [Victor Mono Font](https://rubjo.github.io/victor-mono/)

## Installation

You can either install all of the dependencies listed above by doing it manually or you can type this in your terminal, if you're using an Arch Linux system;
```bash
sudo yay -S alacritty flameshot i3-gaps i3lock-color picom-ibhagwan-git polybar pywal rofi font-victor-mono
```

When this is done;
```bash
git clone https://github.com/archlan/i3-skel.git
```

Then, copy all the files to their appropriate locations.

## Keybinds
> The following table lists all the keybindings for this current setup.

> The `Mod` key here is referred as `$kyoto`, to make modifications easier.

| Keybinds                | Function                |
| ----------------------- | ----------------------- |
| Super Key               | Mod                     |
| $kyoto + L              | Lock the screen         |
| $kyoto + Return         | Open $term              |
| $kyoto                  | Open launcher           |
| $kyoto + 1 2 3 4 5      | Switch workspace        |
| $kyoto + R              | Toggle resize mode      |
| $kyoto + W / Alt + F4   | Kill window             |
| $kyoto + C              | Open wallpaper menu     |
| $kyoto + D              | Open runner             |
| $kyoto + F              | Toggle fullscreen       |
| $kyoto + ← ↑ ↓ →        | Move focus to window    |
| $kyoto + Shift + 1...   | Switch client workspace |
| $kyoto + Shift + R      | Restart i3              |
| Ctrl + Mod1 + Tab       | Flameshot screenshot    |
| $kyoto + Shift + ← ↑ ↓ →| Move focused window     |
| ← ↑ ↓ → (while resize)  | Resize window           |
