i3lock - improved screen locker
===============================

[![Join the chat at https://gitter.im/droserasprout/i3lock](https://badges.gitter.im/droserasprout/i3lock.svg)](https://gitter.im/droserasprout/i3lock?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
i3lock is a simple screen locker like slock. After starting it, you will
see a white screen (you can configure the color/an image). You can return
to your screen by entering your password.

Many little improvements have been made to i3lock over time:

- i3lock forks, so you can combine it with an alias to suspend to RAM
  (run "i3lock && echo mem > /sys/power/state" to get a locked screen
   after waking up your computer from suspend to RAM)

- You can specify either a background color or a PNG image which will be
  displayed while your screen is locked.

- You can specify whether i3lock should bell upon a wrong password.

- You can specify i3lock to logout from any TTYs

- You can run any password-failure script

- You can lock/unlock screen using control socket, if i3lock runs as daemon.
  This feature allow you to lock screen and ttys plug-in (unlock) or plug-out (lock) any device trough USB using UDEV-RULES see z99-lockscreen.rules-example

- i3lock uses PAM and therefore is compatible with LDAP etc.

Requirements
------------
- pkg-config
- libxcb
- libxcb-util
- libpam-dev
- libcairo-dev
- libxcb-xinerama
- libev
- libx11-dev
- libx11-xcb-dev
- libxkbcommon >= 0.5.0
- libxkbcommon-x11 >= 0.5.0

Running i3lock
-------------
Simply invoke the 'i3lock' command. To get out of it, enter your password and
press enter.

Upstream
--------
Please submit pull requests to https://github.com/i3/i3lock
