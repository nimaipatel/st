# st - simple terminal
Nimai's fork of the simple terminal

## Build
```
$ cd ~/some/where
$ git clone https://github.com/nimaipatel/st.git
$ cd st
$ sudo make clean install && make clean
```

## Features
- Live reload colors and font for terminal sessions (kinda like alacritty) using signals and Xresources -- check out this [reddit post](https://www.reddit.com/r/suckless/comments/mew0pt/live_reload_colors_for_st_neovim_dwm_dmenu/) ([credits](https://github.com/gnotclub/xst))
- Quickly copy the output of a shell command with `alt+o` ([credits](https://github.com/lukesmithxyz/st))
- Open URLs in the web browser with `alt+l` and copy them to your clipboard with `alt+c` 
- Transparent background -- requires a compositor, I use this [fork of picom](https://github.com/jonaburg/picom) which also has a cool blur effect
- Spawn new terminal in same working directory as current one with `ctrl+shift+enter`
- Mouse scrollback
- Fallback fonts (set to Joypixels and Nerd Fonts)
- Ligatures -- I don't personally use ligatured fonts but I guess its nice to have the feature?
- Text reflow
- Actual bold fonts instead of just using bright colors

## Dependencies
- [`libxft-bgra`](https://aur.archlinux.org/packages/libxft-bgra-git/) to render color emojis without letting st crash
- [`harfbuzz`](https://archlinux.org/packages/extra/x86_64/harfbuzz/) library for rendering ligatures

## Optional Dependencies
- dmenu to copy and follow URLs and to copy command output
- JoyPixels and Nerd Fonts packages to render color emojis and powerline fonts
- A compositor for transparency and blur effects
