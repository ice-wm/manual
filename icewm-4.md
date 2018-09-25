---
title: Focus models - IceWM Manual
---

[Prev](icewm-3.html) [Top](icewm-toc.html) [Next](icewm-5.html)

Focus models
============

IceWM implements four general focus models:

- **clickToRaise**

  Exactly like Win95, OS/2 Warp. When window is clicked with a mouse, it is raised and activated.

- **clickToFocus**

  Window is raised and focused when titlebar or frame border is clicked. Window is focused but not raised when window interior is clicked.

- **pointerFocus**

  When the mouse is moved, focus is set to window under a mouse. It should be possible to change focus with the keyboard when mouse is not moved.

- **explicitFocus**

  When a window is clicked, it is activated, but not raised. New windows do not automatically get the focus unless they are transient windows for the active window.

Detailed configuration is possible using the configuration file options.

[Prev](icewm-3.html) [Top](icewm-toc.html) [Next](icewm-5.html)
