---
title: The Resource Path - IceWM Manual
---

[Prev](icewm-6.html) [Top](icewm-toc.html) [Next](icewm-8.html)

The Resource Path
=================

IceWM looks in several locations for configuration information, themes and customization; together these locations are called the resource path. The resource path contains the following directories:

$ICEWM\_PRIVCFG; $XDG\_CONFIG\_HOME/icewm; $HOME/.icewm
The first of these which is defined and existent is used to search for the user's personal customization.

/etc/icewm
the system-wide defaults directory

/usr/share/icewm OR /usr/local/share/icewm
the compiled-in default directory with default files

The directories are searched in the above order, so any file located in the system/install directory can be overridden by the user by creating the same directory hierarchy under `$HOME/.icewm`.

To customize icewm yourself, you could create the `$HOME/.icewm` directory and copy the files that you wish to modify, like `preferences`, `keys` or `winoptions`, from `/etc/icewm`, `/usr/share/icewm` or `/usr/local/share/icewm` and then modify as you like.

To customize the default themes, create the `$HOME/.icewm/themes` directory and copy all the theme files there and then modify as necessary. Each theme has its own subdirectory. Themes can be downloaded from <https://www.box-look.org/>.

[Prev](icewm-6.html) [Top](icewm-toc.html) [Next](icewm-8.html)
