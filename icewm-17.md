---
title: Themes - IceWM Manual
---

[Prev](icewm-16.html) [Top](icewm-toc.html) [Next](icewm-18.html)

Themes
======

Themes are used to configure the way the window manager looks. Things like fonts, colors, border sizes, button pixmaps can be configured. Put together they form a theme.

Theme files are searched in the `themes` subdirectories.

These directories contain other directories that contain related theme files and their .xpm files. Each theme file specifies fonts, colors, border sizes, ...

The theme to use is specified in `~/.icewm/theme` file:

- `Theme = "nice/default.theme"`

  Name of the theme to use. Both the directory and theme file name must be specified.

If the theme directory contains a file named *fonts.dir* created by mkfontdir the theme directory is inserted into the X servers font search path.

[www.box-look.org](https://www.box-look.org/browse/cat/142/ord/latest/) has a very large number of themes which were created by users of IceWM.

[Prev](icewm-16.html) [Top](icewm-toc.html) [Next](icewm-18.html)
