# gtk-accent
Bash script to switch Adwaita accent colours on GNOME.

Uses ~/.config/gtk-*n*.0/gtk.css to add shades of the accent as the headerbar colour.

Requires [adw-gtk](https://github.com/lassekongo83/adw-gtk3) and its dark variant to be installed.

Includes options for colouring the terminal prompt, toggling dark / light mode and not theming headerbars.

## Installation:
Run `./gtk-accent setup` from wherever you copy the script to.

This backs up any gtk.css files, generates a new one and creates symlinks to it.\
It also adds a function to .bashrc for setting prompt colour.
### Usage: `gtk-accent [OPTION(S)] [COLOUR]`
```
   -n  Don't theme headerbars
   -P  Theme terminal prompt
   -T  Set theme to dark or light
   -l  List current config and exit
setup  Copy over new gtk.css, create symlinks and exit
```
### Valid colours:
```
       blue, teal, green, yellow, orange,
       red, pink, purple, slate, nautilus
```
