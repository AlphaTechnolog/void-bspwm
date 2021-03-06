<!-- inspired by rxyhn's readme -->

<!-- RICE PREVIEW -->
<div align="center">
   <a href="#--------">
      <img src="assets/banner.png" alt="Rice Preview">
   </a>
</div>

<br>

<!-- BADGES -->
<h1>
  <a href="#--------">
    <img alt="" align="left" src="https://img.shields.io/github/stars/AlphaTechnolog/void-bspwm?color=f1cf8a&labelColor=f1cf8a&style=for-the-badge"/>
  </a>
  <a href="#--------">
    <img alt="" align="right" src="https://badges.pufler.dev/visits/AlphaTechnolog/void-bspwm?style=for-the-badge&color=7ddac5&logoColor=white&labelColor=7ddac5"/>
  </a>
</h1>

<br>

## Hi there! Thanks for dropping by! :green_heart:
<b>  AlphaTechnolog's Void Linux Themed Rice  </b>

Welcome! This is the repository for my void linux themed rice using bspwm + eww!

<!-- INFORMATION -->
## ‎ <samp>Information</samp> 

Here are some details about my setup:

- **OS:** [Void Linux](https://voidlinux.org)
- **WM:** [bspwm](https://github.com/baskerville/bspwm)
- **Terminal:** [st](https://st.suckless.org/)
- **Shell:** [fish](https://fishshell.com/)
- **Editor:** [neovim](https://github.com/neovim/neovim)
- **Compositor:** [picom](https://github.com/yshui/picom)
- **Application Launcher:** [rofi](https://github.com/davatorium/rofi)

<!-- SETUP -->
## ‎ <samp>Setup</samp>

First clone the repository

```sh
git clone https://github.com/AlphaTechnolog/void-bspwm
cd void-bspwm
```

Then install the next requirements

- bspwm
- sxhkd
- picom
- fish
- starship
- eww
- dunst
- rofi
- light
- wireless_tools (for iwgetid)
- alsa-tools (for amixer)
- pulseaudio-alsa
- playerctl

Then copy the configs

**WARNING**: Configuration files may be overrided.

```sh
cp -r ./cfg/* ~/.config
cp -r ./bin/* ~/.local/bin
```

Then compile my build of st (this is the default terminal, but you can change it in the sxhkd configuration):

```sh
cd ~/.config/st
rm config.h && sudo make clean install
```

> It could throws some errors, make sure you have the correct dependencies for st like `harfbuzz` and `imlib2` (if not luck, try installing the `-dev` or `-devel` pkgs)
