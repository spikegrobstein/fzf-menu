# fzf-menu

A quick and dirty script to replace `dmenu`, an i3 app launcher, using `fzf`

## Getting started

 1. Make sure you have `fzf` installed (https://github.com/junegunn/fzf).
 2. Clone this repo somewhere useful.
 3. Edit your i3 config (`~/.config/i3/config`?)

Add the following 2 lines:

    bindsym $mod+space exec termite --class "fzf-menu" --geometry 640x480 -e /path/to/repo/fzf-menu
    for_window [class="^fzf-menu$"] floating enable

The above config usees `termite` as the terminal emulator. You may be able to replace that with the terminal
of your choice.

Be sure to replace `/path/to/repo/fzf-menu` with the path to the `fzf-menu` executable in this repo.

Now, you're good to go! Just press <MOD> + <space> to fire up the launcher!

## Credit

This script was inspired by, and the config basically taken from
http://theinfiniteset.net/2016/02/15/uniting-interfaces-dmenu-and-fzf/

Repository owned by and script itself written by Spike Grobstein (me@spike.cx)

