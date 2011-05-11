# Synopsis

Very dirty hack to allow basic control of Spotify for Linux (play/pause, next, previous), possibly using multimedia keys.

This works by finding the Spotify window and sending appropriate key stokes (this requires it to be temporarily un-minimized, I said it was a hack!)

Forgetting to pause Spotify was driving me mad and this temporary solution seems to do the trick for now

# Requirements

`sudo aptitude install xwit xvkbd wmctrl`
