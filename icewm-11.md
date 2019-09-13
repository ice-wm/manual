---
title: Theme Settings - IceWM Manual
---

[Prev](icewm-10.html) [Top](icewm-toc.html) [Next](icewm-12.html)

Theme Settings
==============

This section shows settings that can be set in theme files. They can also be set in `preferences` file but themes will override the values set there. To override the theme values the settings should be set in `prefoverride` file. Default values are shown following the equal sign.

- `ThemeAuthor =`

  Theme author, e-mail address, credits.

- `ThemeDescription =`

  Description of the theme, credits.

- `Gradients =`

  List of gradient pixmaps in the current theme.

Borders
-------

The following settings can be set to a numeric value.

- `BorderSizeX = 6`

  Left/right border width.

- `BorderSizeY = 6`

  Top/bottom border height.

- `DlgBorderSizeX = 2`

  Left/right border width of non-resizable windows.

- `DlgBorderSizeY = 2`

  Top/bottom border height of non-resizable windows.

- `CornerSizeX = 24`

  Width of the window corner.

- `CornerSizeY = 24`

  Height of the window corner.

- `TitleBarHeight = 20`

  Height of the title bar.

- `TitleBarJustify = 0`

  Justification of the window title.

- `TitleBarHorzOffset = 0`

  Horizontal offset for the window title text.

- `TitleBarVertOffset = 0`

  Vertical offset for the window title text.

- `TitleBarCentered = 0`

  Draw window title centered (obsoleted by TitleBarJustify)

- `TitleBarJoinLeft = 0`

  Join title\*S and title\*T

- `TitleBarJoinRight = 0`

  Join title\*T and title\*B

- `ScrollBarX = 16`

  Scrollbar width.

- `ScrollBarY = 16`

  Scrollbar (button) height.

- `MenuIconSize = 16`

  Menu icon size.

- `SmallIconSize = 16`

  Dimension of the small icons.

- `LargeIconSize = 32`

  Dimension of the large icons.

- `HugeIconSize = 48`

  Dimension of the large icons.

- `QuickSwitchHorzMargin = 3`

  Horizontal margin of the quickswitch window.

- `QuickSwitchVertMargin = 3`

  Vertical margin of the quickswitch window.

- `QuickSwitchIconMargin = 4`

  Vertical margin in the quickswitch window.

- `QuickSwitchIconBorder = 2`

  Distance between the active icon and it's border.

- `QuickSwitchSeparatorSize = 6`

  Height of the separator between (all reachable) icons and text, 0 to avoid it.

- `ShowMenuButtonIcon = 1`

  Show application icon over menu button.

- `TitleButtonsLeft = "s"`

  Titlebar buttons from left to right (x=close, m=max, i=min, h=hide, r=rollup, s=sysmenu, d=depth).

- `TitleButtonsRight = "xmir"`

  Titlebar buttons from right to left (x=close, m=max, i=min, h=hide, r=rollup, s=sysmenu, d=depth).

- `TitleButtonsSupported = "xmis"`

  Titlebar buttons supported by theme (x,m,i,r,h,s,d).

Fonts
-----

The following settings can be set to a string value.

- `TitleFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the title bar font.

- `MenuFontName = "-*-sans-bold-r-*-*-*-100-*-*-*-*-*-*"`

  Name of the menu font.

- `StatusFontName = "-*-monospace-bold-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the status display font.

- `QuickSwitchFontName = "-*-monospace-bold-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the font for Alt+Tab switcher window.

- `NormalButtonFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the normal button font.

- `ActiveButtonFontName = "-*-sans-bold-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the active button font.

- `NormalTaskBarFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the normal task bar item font.

- `ActiveTaskBarFontName = "-*-sans-bold-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the active task bar item font.

- `ToolButtonFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the tool button font (fallback: NormalButtonFontName).

- `NormalWorkspaceFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the normal workspace button font (fallback: NormalButtonFontName).

- `ActiveWorkspaceFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the active workspace button font (fallback: ActiveButtonFontName).

- `MinimizedWindowFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the mini-window font.

- `ListBoxFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the window list font.

- `ToolTipFontName = "-*-sans-medium-r-*-*-*-120-*-*-*-*-*-*"`

  Name of the tool tip font.

- `ClockFontName = "-*-monospace-medium-r-*-*-*-140-*-*-*-*-*-*"`

  Name of the task bar clock font.

- `TempFontName = "-*-monospace-medium-r-*-*-*-140-*-*-*-*-*-*"`

  Name of the task bar temperature font.

- `ApmFontName = "-*-monospace-medium-r-*-*-*-140-*-*-*-*-*-*"`

  Name of the task bar battery font.

- `InputFontName = "-*-monospace-medium-r-*-*-*-140-*-*-*-*-*-*"`

  Name of the input field font.

- `LabelFontName = "-*-sans-medium-r-*-*-*-140-*-*-*-*-*-*"`

  Name of the label font.

When IceWM is configured with `--enable-xfreetype`, only the settings with "Xft" suffix will be used. They specifiy the font name in fontconfig format:

    MenuFontNameXft="sans-serif:size=12:bold"

- `TitleFontNameXft = "sans-serif:size=12"`

  Name of the title bar font.

- `MenuFontNameXft = "sans-serif:size=10:bold"`

  Name of the menu font.

- `StatusFontNameXft = "monospace:size=12:bold"`

  Name of the status display font.

- `QuickSwitchFontNameXft = "monospace:size=12:bold"`

  Name of the font for Alt+Tab switcher window.

- `NormalButtonFontNameXft = "sans-serif:size=12"`

  Name of the normal button font.

- `ActiveButtonFontNameXft = "sans-serif:size=12:bold"`

  Name of the active button font.

- `NormalTaskBarFontNameXft = "sans-serif:size=12"`

  Name of the normal task bar item font.

- `ActiveTaskBarFontNameXft = "sans-serif:size=12:bold"`

  Name of the active task bar item font.

- `ToolButtonFontNameXft = "sans-serif:size=12"`

  Name of the tool button font (fallback: NormalButtonFontNameXft).

- `NormalWorkspaceFontNameXft = "sans-serif:size=12"`

  Name of the normal workspace button font (fallback: NormalButtonFontNameXft).

- `ActiveWorkspaceFontNameXft = "sans-serif:size=12"`

  Name of the active workspace button font (fallback: ActiveButtonFontNameXft).

- `MinimizedWindowFontNameXft = "sans-serif:size=12"`

  Name of the mini-window font.

- `ListBoxFontNameXft = "sans-serif:size=12"`

  Name of the window list font.

- `ToolTipFontNameXft = "sans-serif:size=12"`

  Name of the tool tip font.

- `ClockFontNameXft = "monospace:size=12"`

  Name of the task bar clock font.

- `TempFontNameXft = "monospace:size=12"`

  Name of the task bar temperature font.

- `ApmFontNameXft = "monospace:size=12"`

  Name of the task bar battery font.

- `InputFontNameXft = "monospace:size=12"`

  Name of the input field font.

- `LabelFontNameXft = "sans-serif:size=12"`

  Name of the label font.

Colors
------

- `ColorDialog = "rgb:C0/C0/C0"`

  Background of dialog windows.

- `ColorNormalBorder = "rgb:C0/C0/C0"`

  Border of inactive windows.

- `ColorActiveBorder = "rgb:C0/C0/C0"`

  Border of active windows.

- `ColorNormalButton = "rgb:C0/C0/C0"`

  Background of regular buttons.

- `ColorNormalButtonText = "rgb:00/00/00"`

  Textcolor of regular buttons.

- `ColorActiveButton = "rgb:E0/E0/E0"`

  Background of pressed buttons.

- `ColorActiveButtonText = "rgb:00/00/00"`

  Textcolor of pressed buttons.

- `ColorNormalTitleButton = "rgb:C0/C0/C0"`

  Background of titlebar buttons.

- `ColorNormalTitleButtonText = "rgb:00/00/00"`

  Textcolor of titlebar buttons.

- `ColorToolButton = ""`

  Background of toolbar buttons, ColorNormalButton is used if empty.

- `ColorToolButtonText = ""`

  Textcolor of toolbar buttons, ColorNormalButtonText is used if empty.

- `ColorNormalWorkspaceButton = ""`

  Background of workspace buttons, ColorNormalButton is used if empty.

- `ColorNormalWorkspaceButtonText = ""`

  Textcolor of workspace buttons, ColorNormalButtonText is used if empty.

- `ColorActiveWorkspaceButton = ""`

  Background of the active workspace button, ColorActiveButton is used if empty.

- `ColorActiveWorkspaceButtonText = ""`

  Textcolor of the active workspace button, ColorActiveButtonText is used if empty.

- `ColorNormalTitleBar = "rgb:80/80/80"`

  Background of the titlebar of regular windows.

- `ColorNormalTitleBarText = "rgb:00/00/00"`

  Textcolor of the titlebar of regular windows.

- `ColorNormalTitleBarShadow = ""`

  Textshadow of the titlebar of regular windows.

- `ColorActiveTitleBar = "rgb:00/00/A0"`

  Background of the titlebar of active windows.

- `ColorActiveTitleBarText = "rgb:FF/FF/FF"`

  Textcolor of the titlebar of active windows.

- `ColorActiveTitleBarShadow = ""`

  Textshadow of the titlebar of active windows.

- `ColorNormalMinimizedWindow = "rgb:C0/C0/C0"`

  Background for mini icons of regular windows.

- `ColorNormalMinimizedWindowText = "rgb:00/00/00"`

  Textcolor for mini icons of regular windows.

- `ColorActiveMinimizedWindow = "rgb:E0/E0/E0"`

  Background for mini icons of active windows.

- `ColorActiveMinimizedWindowText = "rgb:00/00/00"`

  Textcolor for mini icons of active windows.

- `ColorNormalMenu = "rgb:C0/C0/C0"`

  Background of pop-up menus.

- `ColorNormalMenuItemText = "rgb:00/00/00"`

  Textcolor of regular menu items.

- `ColorActiveMenuItem = "rgb:A0/A0/A0"`

  Background of selected menu item, leave empty to force transparency.

- `ColorActiveMenuItemText = "rgb:00/00/00"`

  Textcolor of selected menu items.

- `ColorDisabledMenuItemText = "rgb:80/80/80"`

  Textcolor of disabled menu items.

- `ColorDisabledMenuItemShadow = ""`

  Shadow of regular menu items.

- `ColorMoveSizeStatus = "rgb:C0/C0/C0"`

  Background of move/resize status window.

- `ColorMoveSizeStatusText = "rgb:00/00/00"`

  Textcolor of move/resize status window.

- `ColorQuickSwitch = "rgb:C0/C0/C0"`

  Background of the quick switch window.

- `ColorQuickSwitchText = "rgb:00/00/00"`

  Textcolor in the quick switch window.

- `ColorQuickSwitchActive = ""`

  Rectangle arround the active icon in the quick switch window.

- `ColorDefaultTaskBar = "rgb:C0/C0/C0"`

  Background of the taskbar.

- `ColorNormalTaskBarApp = "rgb:C0/C0/C0"`

  Background for task buttons of regular windows.

- `ColorNormalTaskBarAppText = "rgb:00/00/00"`

  Textcolor for task buttons of regular windows.

- `ColorActiveTaskBarApp = "rgb:E0/E0/E0"`

  Background for task buttons of the active window.

- `ColorActiveTaskBarAppText = "rgb:00/00/00"`

  Textcolor for task buttons of the active window.

- `ColorMinimizedTaskBarApp = "rgb:A0/A0/A0"`

  Background for task buttons of minimized windows.

- `ColorMinimizedTaskBarAppText = "rgb:00/00/00"`

  Textcolor for task buttons of minimized windows.

- `ColorInvisibleTaskBarApp = "rgb:80/80/80"`

  Background for task buttons of windows on other workspaces.

- `ColorInvisibleTaskBarAppText = "rgb:00/00/00"`

  Textcolor for task buttons of windows on other workspaces.

- `ColorScrollBar = "rgb:A0/A0/A0"`

  Scrollbar background (sliding area).

- `ColorScrollBarSlider = "rgb:C0/C0/C0"`

  Background of the slider button in scrollbars.

- `ColorScrollBarButton = "rgb:C0/C0/C0"`

  Background of the arrow buttons in scrollbars.

- `ColorScrollBarArrow = "rgb:C0/C0/C0"`

  Background of the arrow buttons in scrollbars (obsolete).

- `ColorScrollBarButtonArrow = "rgb:00/00/00"`

  Color of active arrows on scrollbar buttons.

- `ColorScrollBarInactiveArrow = "rgb:80/80/80"`

  Color of inactive arrows on scrollbar buttons.

- `ColorListBox = "rgb:C0/C0/C0"`

  Background of listboxes.

- `ColorListBoxText = "rgb:00/00/00"`

  Textcolor in listboxes.

- `ColorListBoxSelection = "rgb:80/80/80"`

  Background of selected listbox items.

- `ColorListBoxSelectionText = "rgb:00/00/00"`

  Textcolor of selected listbox items.

- `ColorToolTip = "rgb:E0/E0/00"`

  Background of tooltips.

- `ColorToolTipText = "rgb:00/00/00"`

  Textcolor of tooltips.

- `ColorLabel = "rgb:C0/C0/C0"`

  Background of labels, leave empty to force transparency.

- `ColorLabelText = "rgb:00/00/00"`

  Textcolor of labels.

- `ColorInput = "rgb:FF/FF/FF"`

  Background of text entry fields (e.g. the addressbar).

- `ColorInputText = "rgb:00/00/00"`

  Textcolor of text entry fields (e.g. the addressbar).

- `ColorInputSelection = "rgb:80/80/80"`

  Background of selected text in an entry field.

- `ColorInputSelectionText = "rgb:00/00/00"`

  Selected text in an entry field.

- `ColorClock = "rgb:00/00/00"`

  Background of non-LCD clock, leave empty to force transparency.

- `ColorClockText = "rgb:00/FF/00"`

  Background of non-LCD monitor.

- `ColorApm = "rgb:00/00/00"`

  Background of APM monitor, leave empty to force transparency.

- `ColorApmText = "rgb:00/FF/00"`

  Textcolor of APM monitor.

- `ColorApmBattary = "rgb:FF/FF/00"`

  Color of APM monitor in battery mode.

- `ColorApmLine = "rgb:00/FF/00"`

  Color of APM monitor in line mode.

- `ColorApmGraphBg = "rgb:00/00/00"`

  Background color for graph mode.

- `ColorCPUStatusUser = "rgb:00/FF/00"`

  User load on the CPU monitor.

- `ColorCPUStatusSystem = "rgb:FF/00/00"`

  System load on the CPU monitor.

- `ColorCPUStatusInterrupts = "rgb:FF/FF/00"`

  Interrupts on the CPU monitor.

- `ColorCPUStatusIoWait = "rgb:60/00/60"`

  IO Wait on the CPU monitor.

- `ColorCPUStatusSoftIrq = "rgb:00/FF/FF"`

  Soft Interrupts on the CPU monitor.

- `ColorCPUStatusNice = "rgb:00/00/FF"`

  Nice load on the CPU monitor.

- `ColorCPUStatusIdle = "rgb:00/00/00"`

  Idle (non) load on the CPU monitor, leave empty to force transparency.

- `ColorCPUStatusSteal = "rgb:FF/8A/91"`

  Involuntary Wait on the CPU monitor.

- `ColorCPUStatusTemp = "rgb:60/60/C0"`

  Temperature of the CPU.

- `ColorMEMStatusUser = "rgb:40/40/80"`

  User program usage in the memory monitor.

- `ColorMEMStatusBuffers = "rgb:60/60/C0"`

  OS buffers usage in the memory monitor.

- `ColorMEMStatusCached = "rgb:80/80/FF"`

  OS cached usage in the memory monitor.

- `ColorMEMStatusFree = "rgb:00/00/00"`

  Free memory in the memory monitor.

- `ColorNetSend = "rgb:FF/FF/00"`

  Outgoing load on the network monitor.

- `ColorNetReceive = "rgb:FF/00/FF"`

  Incoming load on the network monitor.

- `ColorNetIdle = "rgb:00/00/00"`

  Idle (non) load on the network monitor, leave empty to force transparency.

- `ColorApmBattery = rgb:FF/FF/00`

  Color of APM monitor in battery mode.

Desktop Background
------------------

The following options are used by `icewmbg`:

- `DesktopBackgroundCenter = 0`

  Display desktop background centered and not tiled. (set to 0 or 1).

- `DesktopBackgroundScaled = 0`

  Resize desktop background to full screen.

- `DesktopBackgroundColor = ""`

  Color(s) of the desktop background.

- `DesktopBackgroundImage = ""`

  Image(s) for desktop background. If you want IceWM to ignore the desktop background image / color set both DesktopBackgroundColor and DesktopBackgroundImage to an empty value ("").

- `SupportSemitransparency = 1`

  Support for semitransparent terminals like Eterm or gnome-terminal.

- `DesktopTransparencyColor = ""`

  Color(s) to announce for semitransparent windows.

- `DesktopTransparencyImage = ""`

  Image(s) to announce for semitransparent windows.

- `DesktopBackgroundMultihead = 0`

  Paint the background image over all multihead monitors combined.

Task Bar
--------

- `TaskBarClockLeds = 1`

  Display clock using LCD style pixmaps.

[Prev](icewm-10.html) [Top](icewm-toc.html) [Next](icewm-12.html)
