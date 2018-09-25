---
title: Icon handling - IceWM Manual
---

[Prev](icewm-14.html) [Top](icewm-toc.html) [Next](icewm-16.html)

Icon handling
=============

Generic
-------

The window manager expects to find two XPM files for each icon specified in the configuration files as *ICON*. They should be named like this:

- **ICON\_16x16.xpm**

  A small 16x16 pixmap.

- **ICON\_32x32.xpm**

  A normal 32x32 pixmap.

- **ICON\_48x48.xpm**

  A large 48x48 pixmap.

Other pixmap sizes like 20x20, 24x24, 40x40, 48x48, 64x64 might be used in the future. Perhaps we need a file format that can contain more than one image (with different sizes and color depths) like Windows'95 and OS/2 .ICO files.

It would be nice to have a feature from OS/2 that varies the icon size with screen resolution (16x16 and 32x32 icons are quite small on 4000x4000 screens ;-)

GDK-Pixbuf
----------

When icewm was configured with the `--enable-gdk-pixbuf` option all of GdkPixbuf's image formats are supported. Use them by specifying the full filename or an absolute path:

- **ICON.bmp**

  A PPM icon in your IconPath.

- **/usr/share/pixmap/ICON.png**

  An PNG image with absolute location.

[Prev](icewm-14.html) [Top](icewm-toc.html) [Next](icewm-16.html)
