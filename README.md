# Synopsis

Very dirty hack to allow basic control of Spotify for Linux (play/pause, next, previous), possibly using multimedia keys.

This works by finding the Spotify window and sending appropriate key stokes (this requires it to be temporarily un-minimized, I said it was a hack!)

Forgetting to pause Spotify was driving me mad and this temporary solution seems to do the trick for now

# Installation

  - Install dependencies (wxit, xvkbd, wmctrl)
    - On Ubuntu, you can use `sudo aptitude install xwit xvkbd wmctrl`
  - Place the script in an appropriate location, e.g. `~/bin`
  - You can test the script by running it on the command line
    - With no parameters it will send a space keypress, which will play/pause Spotity
    - Otherwise the first parameter specifies the key combination, in `xvkbd` format, e.g.
      - Next - `spotify_keyboard "\C\[Right]"`
      - Previous - `spotify_keyboard "\C\[Left]"`
  - Bind the command to keyboard shortcuts
    - On Gnome, use the 'Keyboard shortcuts' dialogue under 'System', 'Preferences'. Create custom shortcuts and bind to your preferred keys
