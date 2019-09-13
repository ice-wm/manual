---
title: Window Options (updated 2018-03-04) - IceWM Manual
---

[Prev](icewm-13.html) [Top](icewm-toc.html) [Next](icewm-15.html)

Window Options (updated 2018-03-04)
===================================

The **winoptions** file is used to configure settings for individual application windows. Each line in this file must have one of the following formats:

- **  window\_name.window\_class.option: argument**

- **  window\_name.window\_role.option: argument**

- **  window\_class.option: argument**

- **  window\_name.option: argument**

- **  window\_role.option: argument**

- **  .option: argument**

The last format sets a default option value for all windows. Each window on the desktop should have **name** and **class** resources associated with it. Some applications also have a **window role** resource. They can be determined using the `xprop` utility. When used on a toplevel window, `xprop | grep -e CLASS -e ROLE` should output a line like this:

    WM_CLASS = "name", "Class"

and may also display a line like this:

    WM_WINDOW_ROLE = "window role"

It's possible that an application's **name** and/or **class** contains a dot character (**.**), which is also used by IceWM to separate **name**, **class** and **role** values. In this case precede the dot with the backslash character. In the following example, we suppose an application's window has `the.name` as its **name** value and `The.Class` as its **class** value and for this combination we set **option** to **argument**.

    the\.name.The\.Class.option: argument

Options that can be set per window are as follows:

- **icon**

  The name of the icon.

- **workspace**

  Default workspace for window (number, counting from 0)

- **layer**

  The default stacking layer for the window. Layer can be one of the following seven strings:


  - *Desktop*
    Desktop window. There should be only one window in this layer.

  - *Below*
    Below default layer.

  - *Normal*
    Default layer for the windows.

  - *OnTop*
    Above the default.

  - *Dock*
    Layer for windows docked to the edge of the screen.

  - *AboveDock*
    Layer for the windows above the dock.

  - *Menu*
    Layer for the windows above the dock.


  You can also use a number from 0 to 15.

- **geometry**

  The default geometry for the window. This geometry should be specified in the usual X11-geometry-syntax, formal notation:

        [=][<width>{xX}<height>][{+-}<xoffset>{+-}<yoffset>]

- **tray**

  The default tray option for the window. This affects both the tray and the task pane. Tray can be one of the following strings:


  - *Ignore*
    Don't add an icon to the tray pane.

  - *Minimized*
    Add an icon the the tray. Remove the task pane button when minimized.

  - *Exclusive*
    Add an icon the the tray. Never create a task pane button.

- **order: 0**

  The sorting order of task buttons and tray icons. The default value is zero. Increasing positive values go farther right, while decreasing negative values go farther left. The order option applies to the task pane, the tray pane and the system tray.

- **allWorkspaces: 0**

  If set to 1, window will be visible on all workspaces.

- **appTakesFocus: 0**

  if set to 1, IceWM will assume the window supports the WM\_TAKE\_FOCUS protocol even if the window did not advertise that it does.

- **dBorder: 1**

  If set to 0, window will not have a border.

- **dClose: 1**

  If set to 0, window will not have a close button.

- **dDepth: 1**

  If set to 0, window will not have a depth button.

- **dHide: 1**

  If set to 0, window will not have a hide button.

- **dMaximize: 1**

  If set to 0, window will not have a maximize button.

- **dMinimize: 1**

  If set to 0, window will not have a minimize button.

- **dResize: 1**

  If set to 0, window will not have a resize border.

- **dRollup: 1**

  If set to 0, window will not have a shade button.

- **dSysMenu: 1**

  If set to 0, window will not have a system menu.

- **dTitleBar: 1**

  If set to 0, window will not have a title bar.

- **doNotCover: 0**

  if set to 1, this window will limit the workspace available for regular applications. At the moment the window has to be sticky to make it work.

- **doNotFocus: 0**

  if set to 1, IceWM will never give focus to the window.

- **fClose: 1**

  If set to 0, window will not be closable.

- **fHide: 1**

  If set to 0, window will not be hidable.

- **fMaximize: 1**

  If set to 0, window will not be maximizable.

- **fMinimize: 1**

  If set to 0, window will not be minimizable.

- **fMove: 1**

  If set to 0, window will not be movable.

- **fResize: 1**

  If set to 0, window will not be resizable.

- **fRollup: 1**

  If set to 0, window will not be shadable.

- **forcedClose: 0**

  if set to 1 and the application had not registered WM\_DELETE\_WINDOW, a close confirmation dialog won't be offered upon closing the window.

- **fullKeys: 0**

  If set to 1, the window manager leave more keys (Alt+F?) to the application.

- **ignoreNoFocusHint: 0**

  if set to 1, IceWM will focus even if the window does not handle input.

- **ignorePagerPreview: 0**

  If set to 1, window will not appear in pager preview.

- **ignorePositionHint: 0**

  if set to 1, IceWM will ignore the position hint.

- **ignoreQuickSwitch: 0**

  If set to 1, window will not be accessible using QuickSwitch feature (Alt+Tab).

- **ignoreTaskBar: 0**

  If set to 1, window will not appear on the task bar.

- **ignoreUrgentHint: 0**

  if set to 1, IceWM will ignore it if the window sets the urgent hint.

- **ignoreWinList: 0**

  If set to 1, window will not appear in the window list.

- **noFocusOnAppRaise: 0**

  if set to 1, window will not automatically get focus as application raises it.

- **noFocusOnMap: 0**

  if set to 1, IceWM will not assign focus when the window is mapped for the first time.

- **noIgnoreTaskBar: 0**

  if set to 1, will show the window on the taskbar.

- **nonICCCMconfigureRequest: 0**

  if set to 1, IceWM assumes the application does not support the ICCCM standard wrt positioning and compensate for that.

- **startFullscreen: 0**

  if set to 1, window will cover the entire screen.

- **startMaximized: 0**

  if set to 1, window starts maximized.

- **startMaximizedHorz: 0**

  if set to 1, window starts maximized horizontally.

- **startMaximizedVert: 0**

  if set to 1, window starts maximized vertically.

- **startMinimized: 0**

  if set to 1, window starts minimized.

[Prev](icewm-13.html) [Top](icewm-toc.html) [Next](icewm-15.html)
