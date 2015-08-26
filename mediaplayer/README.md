# Media player

Generic media player support

This displays "ARTIST - SONG [- ALBUM]" if music is playing
(album is currently displayed only for MPRIS).
Supported players are:
- spotify, vlc, audacious, xmms2, mplayer and others that
use MPRIS DBus Interface Specification
- mpd
- cmus

mpd is supported through mpc (music player client).

For MPRIS support you need to have playerctl binary in your path.
See: https://github.com/acrisci/playerctl

If you leave the instance empty it will try to find an
active player used on it's own.

Clicking on the block area with left, middle and right click
will cause the player used to pause, jump to previous and
next (can be customized in the script).

``` ini
[mediaplayer]
command=./mediaplayer
instance=spotify
interval=5
signal=10
```
