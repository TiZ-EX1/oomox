﻿oomox
=====

## Graphical application for generating different color variations of Numix theme (GTK2, GTK3)

![Screenshot GUI 1](https://raw.githubusercontent.com/actionless/oomox/master/screenshot_gui.png "Screenshot GUI 1")

![Screenshot GUI 2](https://raw.githubusercontent.com/actionless/oomox/master/screenshot_gui_retro.png "Screenshot GUI 2")

### Arch Linux:

#### Install

```
yaourt -S oomox-git
```

#### GUI

```
oomox-gui
```


### Using with tiling WMs:

To resolve borders/shadow problem in tiling window managers create/append to 
`~/.config/gtk-3.0/gtk.css`:

```css
.window-frame, .window-frame:backdrop {
  box-shadow: 0 0 0 black;
  border-style: none;
  margin: 0;
  border-radius: 0;
}
.titlebar {
  border-radius: 0;
}
window decoration {
	margin: 0;
}
```


### Other distributions:

#### Prerequisites

You need to have `python3-gobject` binding and those executables:
 - `glib-compile-schemas`
 - `gdk-pixbuf-pixdata`
 - `sass`

##### Ubuntu

```
sudo apt install ruby libgdk-pixbuf2.0-dev libxml2-utils python3-gi
sudo gem install sass
```

#### GUI

```sh
git clone https://github.com/actionless/oomox.git
cd oomox
./gui.sh
```

#### CLI:
```sh
git clone https://github.com/actionless/oomox.git
cd oomox
ls colors
./change_color.sh gnome_noble  # or other theme from above
```


next select oomox_current in your appearance config tool (for example, _lxappearance_)

