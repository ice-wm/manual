---
title: First steps - IceWM Manual
---

[Prev](icewm-2.html) [Top](icewm-toc.html) [Next](icewm-4.html)

First steps
===========

IceWM components
----------------

The IceWM suite consists of the following core applications provided by the main package:

-   **[icewm](/man/icewm.html)** - The actual window manager binary. It handles window placement and draws the window decorations.

-   **[icewmbg](/man/icewmbg.html)** - The background setting application. It can assign plain background color or images in different formats to the X background. Either shared or separate for different workspaces. This program should be started before `icewm`.

-   **[icewm-session](/man/icewm-session.html)** - The IceWM session manager runs all of the above. This is the preferred program to start IceWM.

-   **[icewm-menu-fdo](/man/icewm-menu-fdo.html)** - This generates IceWM program menus from FreeDesktop `.desktop` files.

-   **[icewmhint](/man/icewmhint.html)** - Is a simple utility for passing IceWM hints to IceWM by window class and instance. Icewmhint uses a special property, '"\_ICEWM\_WINOPHINT"', on the root window to pass special hints to IceWM.

-   **[icehelp](/man/icehelp.html)** - Is used by icewm to display the 'IceWM manual' and the manpages. See the output of `icehelp --help` for details.

-   **[icesh](/man/icesh.html)** - Could be used to manage IceWM internals from the command line.

Starting icewm
--------------

The `icewm` program alone is suitable for use with desktop environments like GNOME. If you wish to run the whole IceWM suite (WM, background changer, Docklet support, and startup/shutdown script handling), use the `icewm-session` binary instead of pure `icewm`. Note that this is not a complete Session Manager but it helps to automate the startup.

First make sure that you choose the correct [X startup](https://www.tldp.org/HOWTO/XWindow-User-HOWTO/runningx.html) script in your home directory. For most distributions either the file `$HOME/.xsession` or `$HOME/.xinitrc` is honored by startx and X display managers like KDM. On RedHat, the `$HOME/.Xclients` may be used instead. In all cases, choose the one recommended by your distribution and make sure that there is no concurrency between the X startup scripts. Ensure that the script is executable. Mine looks something like this:

    #!/bin/bash
    # run profile to set $PATH and other env vars correctly
    . $HOME/.bash_profile
    # setup touchpad and the external mouse
    xset m 7 2
    xinput set-ptr-feedback 0 7 1.9 1

    # start icewm-session
    exec icewm-session
    xterm

The xterm on the last line is there simply to make sure that your X session doesn't crash if IceWM does (should never happen). You can restart IceWM from there or start some other window manager. The session will close if you close the xterm.

Startup and shutdown scripts
----------------------------

After initialization `icewm-session` will search the resource path for a `startup` script. If this file is found and if it is executable `icewm-session` will run this script. During termination of `icewm-session` the `shutdown` script is executed.

Example `~/.icewm/startup` script:

    #!/bin/bash

    [ -x ~/.icewm/restart ] && source ~/.icewm/restart

    gnome-terminal --geometry 80x25+217+235 &
    xscreensaver &

On termination the `shutdown` script will be run first, then `icewm-session` will terminate icewm and icewmbg.

Hint: `icewm-session` is meant for easy desktop initialization and it is part of IceWM due to popular demand. For more sophisticated session management one could use a real session manager. IceWM supports the XSESSION protocol.

Extra session environment
-------------------------

Please note that if icewm-session is used as the only startup mechanism (without having .xsession involved), one can write additional environment settings into the file `$HOME/.icewm/env`. Expansion of simple shell style variables should be supported on most platforms. Shell command expansion is supported if `wordexp` was configured. This extra environment is only effective in applications started by icewm-session and their subprocesses.

Example `env`:

    PATH=~/bin:$PATH
    LANG=de_DE.UTF-8

[Prev](icewm-2.html) [Top](icewm-toc.html) [Next](icewm-4.html)
