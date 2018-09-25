---
title: Hot Keys - IceWM Manual
---

[Prev](icewm-12.html) [Top](icewm-toc.html) [Next](icewm-14.html)

Hot Keys
========

IceWM allows launching of arbitrary programs with any key combination. This is configured in the `keys` file. The syntax of this file is like:

**key** "key combination" program options...

For example:

    key  "Alt+Ctrl+t"  xterm -rv
    key "Ctrl+Shift+r" icewm --restart
    runonce "Alt+F12"  "res_name.res_class" program_executable options

[Prev](icewm-12.html) [Top](icewm-toc.html) [Next](icewm-14.html)
