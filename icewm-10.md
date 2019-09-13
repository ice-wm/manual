---
title: Preferences - IceWM Manual
---

[Prev](icewm-9.html) [Top](icewm-toc.html) [Next](icewm-11.html)

Preferences
===========

This section shows preferences that can be set in `preferences`. Themes will not be able to override these settings. Default values are shown following the equal sign.

Focus and Behavior
------------------

The following settings can be set to value 1 (enabled) or value 0 (disabled).

- `ClickToFocus = 1`

  Enables click to focus mode.

- `RaiseOnFocus = 1`

  Window is raised when focused.

- `FocusOnClickClient = 1`

  Window is focused when client area is clicked.

- `RaiseOnClickClient = 1`

  Window is raised when client area is clicked.

- `RaiseOnClickTitleBar = 1`

  Window is raised when titlebar is clicked.

- `RaiseOnClickButton = 1`

  Window is raised when title bar button is clicked.

- `RaiseOnClickFrame = 1`

  Window is raised when frame is clicked.

- `LowerOnClickWhenRaised = 0`

  Lower the active window when clicked again.

- `PassFirstClickToClient = 1`

  The click which raises the window is also passed to the client.

- `FocusChangesWorkspace = 0`

  Change to the workspace of newly focused windows.

- `AutoRaise = 0`

  Windows will raise automatically after AutoRaiseDelay when focused.

- `StrongPointerFocus = 0`

  When focus follows mouse always give the focus to the window under mouse pointer - Even when no mouse motion has occurred. Using this is not recommended. Please prefer to use just ClickToFocus=0.

- `FocusOnMap = 1`

  Window is focused after being mapped.

- `FocusOnMapTransient = 1`

  Transient window is focused after being mapped.

- `FocusOnMapTransientActive = 1`

  Focus dialog window when initially mapped only if parent frame focused.

- `FocusOnAppRaise = 1`

  The window is focused when application raises it.

- `RequestFocusOnAppRaise = 1`

  Request focus (flashing in taskbar) when application requests raise.

- `MapInactiveOnTop = 1`

  Put new windows on top even if not focusing them.

- `PointerColormap = 0`

  Colormap focus follows pointer.

- `DontRotateMenuPointer = 1`

  Don't rotate the cursor for popup menus.

- `LimitSize = 1`

  Limit size of windows to screen.

- `LimitPosition = 1`

  Limit position of windows to screen.

- `LimitByDockLayer = 0`

  Let the Dock layer limit the workspace (incompatible with GNOME Panel).

- `ConsiderHBorder = 0`

  Consider border frames when maximizing horizontally.

- `ConsiderVBorder = 0`

  Consider border frames when maximizing vertically.

- `ConsiderSizeHintsMaximized = 1`

  Consider XSizeHints if frame is maximized.

- `CenterMaximizedWindows = 0`

  Center maximized windows which can't fit the screen (like terminals).

- `HideBordersMaximized = 0`

  Hide window borders if window is maximized.

- `HideTitleBarWhenMaximized = 0`

  Hide title bar when maximized.

- `CenterLarge = 0`

  Center large windows.

- `CenterTransientsOnOwner = 1`

  Center dialogs on owner window.

- `SizeMaximized = 0`

  Window can be resized when maximized.

- `MinimizeToDesktop = 0`

  Window is minimized to desktop area (in addition to the taskbar).

- `MiniIconsPlaceHorizontal = 0`

  Place the mini-icons horizontal instead of vertical.

- `MiniIconsRightToLeft = 0`

  Place new mini-icons from right to left.

- `MiniIconsBottomToTop = 0`

  Place new mini-icons from bottom to top.

- `GrabRootWindow = 1`

  Manage root window (EXPERIMENTAL - normally enabled!).

- `ShowMoveSizeStatus = 1`

  Move/resize status window is visible when moving/resizing the window.

- `ShowWorkspaceStatus = 1`

  Show name of current workspace while switching.

- `ShowWorkspaceStatusAfterSwitch = 1`

  Show name of current workspace while switching workspaces.

- `ShowWorkspaceStatusAfterActivation = 1`

  Show name of current workspace after explicit activation.

- `WarpPointer = 0`

  Pointer is moved in pointer focus move when focus is moved using the keyboard.

- `OpaqueMove = 1`

  Window is immediately moved when dragged, no outline is shown.

- `OpaqueResize = 0`

  Window is immediately resized when dragged, no outline is shown.

- `DelayPointerFocus = 1`

  Similar to delayed auto raise.

- `Win95Keys = 0`

  Makes 3 additional keys perform sensible functions. The keys must be mapped to MetaL, MetaR and Menu. The left one will activate the start menu and the right one will display the window list.

- `ModSuperIsCtrlAlt = 1`

  Treat Super/Win modifier as Ctrl+Alt.

- `UseMouseWheel = 0`

  mouse wheel support

- `ShowPopupsAbovePointer = 0`

  Show popup menus above mouse pointer.

- `ReplayMenuCancelClick = 0`

  Send the clicks outside menus to target window.

- `ManualPlacement = 0`

  Windows must be placed manually by the user.

- `SmartPlacement = 1`

  Smart window placement (minimal overlap).

- `IgnoreNoFocusHint = 0`

  Ignore no-accept-focus hint set by some windows.

- `MenuMouseTracking = 0`

  If enabled, menus will track the mouse even when no mouse button is pressed.

- `ClientWindowMouseActions = 1`

  Allow mouse actions on client windows.

- `SnapMove = 1`

  Snap to nearest screen edge/window when moving windows.

- `SnapDistance = 8`

  Distance in pixels before windows snap together

- `ArrangeWindowsOnScreenSizeChange = 1`

  Automatically arrange windows when screen size changes.

- `MsgBoxDefaultAction = 0`

  Preselect to Cancel (0) or the OK (1) button in message boxes

- `EdgeResistance = 32`

  Resistance to move window with mouse outside screen limits. Setting it to 10000 makes the resistance infinite.

- `AllowFullscreen = 1`

  Allow to switch a window to fullscreen.

- `FullscreenUseAllMonitors = 0`

  Span over all available screens if window goes into fullscreen.

- `NetWorkAreaBehaviour = 0`

  NET\_WORKAREA behaviour: 0 (single/multimonitor with STRUT information, like metacity), 1 (always full desktop), 2 (singlemonitor with STRUT, multimonitor without STRUT).

- `ConfirmLogout = 1`

  Confirm Logout.

- `MultiByte = 1`

  Overrides automatic multiple byte detection.

- `ShapesProtectClientWindow = 1`

  Don't cut client windows by shapes set trough frame corner pixmap.

- `DoubleBuffer = 1`

  Use double buffering when redrawing the display.

- `XRRDisable = 0`

  Disable use of new XRANDR API for dual head (nvidia workaround)

- `PreferFreetypeFonts = 1`

  Favor \*Xft fonts over core X11 fonts where possible.

- `IconPath = /usr/share/icons/hicolor:/usr/share/icons:/usr/share/pixmaps`

  Icon search path (colon separated)

- `MailCommand = xterm -name mutt -e mutt`

  Command to run on mailbox.

- `MailClassHint = mutt.XTerm`

  WM\_CLASS to allow runonce for MailCommand.

- `LockCommand =`
  Command to lock display/screensaver.

- `ClockCommand = xclock -name icewm -title Clock`

  Command to run on clock.

- `ClockClassHint = icewm.XClock`

  WM\_CLASS to allow runonce for ClockCommand.

- `RunCommand =`
  Command to select and run a program.

- `OpenCommand =`
  Command to run to open a file.

- `TerminalCommand = xterm`

Terminal emulator must accept -e option.

- `LogoutCommand =`
  Command to start logout.

- `LogoutCancelCommand =`
  Command to cancel logout.

- `ShutdownCommand =`
  Command to shutdown the system.

- `RebootCommand =`
  Command to reboot the system.

- `SuspendCommand =`
  Command to send the system to standby mode.

- `CPUStatusCommand =`
  Command to run on CPU status.

- `CPUStatusClassHint = top.XTerm`

  WM\_CLASS to allow runonce for CPUStatusCommand.

- `CPUStatusCombine = 1`

  Combine all CPUs to one.

- `NetStatusCommand =`
  Command to run on Net status.

- `NetStatusClassHint = netstat.XTerm`

  WM\_CLASS to allow runonce for NetStatusCommand.

- `AddressBarCommand =`
  Command to run for address bar entries.

- `XRRPrimaryScreenName =`
  screen/output name of the primary screen.

### Quick Switch List

- `QuickSwitch = 1`

  enable Alt+Tab window switcher.

- `QuickSwitchToMinimized = 1`

  Alt+Tab switches to minimized windows too.

- `QuickSwitchToHidden = 1`

  Alt+Tab to hidden windows.

- `QuickSwitchToUrgent = 1`

  Prioritize Alt+Tab to urgent windows.

- `QuickSwitchToAllWorkspaces = 1`

  Alt+Tab switches to windows on any workspace.

- `QuickSwitchGroupWorkspaces = 1`

  Alt+Tab: group windows on current workspace.

- `QuickSwitchAllIcons = 1`

  Show all reachable icons when quick switching.

- `QuickSwitchTextFirst = 0`

  Show the window title above (all reachable) icons.

- `QuickSwitchSmallWindow = 0`

  Attempt to create a small QuickSwitch window (1/3 instead of 3/5 of

- `QuickSwitchMaxWidth = 0`

  Go through all window titles and choose width of the longest one.

- `QuickSwitchVertical = 1`

  Place the icons and titles vertical instead of horizontal.

- `QuickSwitchHugeIcon = 0`

  Show the huge (48x48) of the window icon for the active window.

- `QuickSwitchFillSelection = 0`

  Fill the rectangle highlighting the current icon.

### Edge Workspace Switching

- `EdgeSwitch = 0`

  Workspace switches by moving mouse to left/right screen edge.

- `HorizontalEdgeSwitch = 0`

  Workspace switches by moving mouse to left/right screen edge.

- `VerticalEdgeSwitch = 0`

  Workspace switches by moving mouse to top/bottom screen edge.

- `ContinuousEdgeSwitch = 1`

  Workspace switches continuously when moving mouse to screen edge.

Task Bar
--------

The following settings can be set to value 1 (enabled) or value 0 (disabled).

- `ShowTaskBar = 1`

  Task bar is visible.

- `TaskBarAtTop = 0`

  Task bar is located at top of screen.

- `TaskBarKeepBelow = 1`

  Keep the task bar below regular windows

- `TaskBarAutoHide = 0`

  Task bar will auto hide when mouse leaves it.

- `TaskBarFullscreenAutoShow = 1`

  Auto show task bar when fullscreen window active.

- `TaskBarShowClock = 1`

  Task bar clock is visible.

- `TaskBarShowAPMStatus = 0`

  Show APM/ACPI/Battery/Power status monitor on task bar.

- `TaskBarShowAPMAuto = 1`

  Enable TaskBarShowAPMStatus if a battery is present.

- `TaskBarShowAPMTime = 1`

  Show APM status on task bar in time-format.

- `TaskBarShowAPMGraph = 1`

  Show APM status in graph mode.

- `TaskBarShowMailboxStatus = 1`

  Display status of mailbox (see 'Mailbox' below).

- `TaskBarMailboxStatusBeepOnNewMail = 0`

  Beep when new mail arrives.

- `TaskBarMailboxStatusCountMessages = 0`

  Display mail message count as tooltip.

- `TaskBarShowWorkspaces = 1`

  Show workspace switching buttons on task bar.

- `TaskBarShowWindows = 1`

  Show windows on the taskbar.

- `TaskBarShowShowDesktopButton = 1`

  Show 'show desktop' button on taskbar.

- `ShowEllipsis = 0`

  Show Ellipsis in taskbar items.

- `TaskBarShowTray = 1`

  Show windows in the tray.

- `TrayShowAllWindows = 1`

  Show windows from all workspaces on tray.

- `TaskBarEnableSystemTray = 1`

  Enable the system tray in the taskbar.

- `TaskBarShowTransientWindows = 1`

  Show transient (dialogs, ...) windows on task bar.

- `TaskBarShowAllWindows = 0`

  Show windows from all workspaces on task bar.

- `TaskBarShowWindowIcons = 1`

  Show icons of windows on the task bar.

- `TaskBarShowStartMenu = 1`

  Show button for the start menu on the task bar.

- `TaskBarShowWindowListMenu = 1`

  Show button for window list menu on taskbar.

- `TaskBarShowCPUStatus = 1`

  Show CPU status on task bar (Linux & Solaris).

- `CPUStatusShowRamUsage = 1`

  Show RAM usage in CPU status tool tip.

- `CPUStatusShowSwapUsage = 1`

  Show swap usage in CPU status tool tip.

- `CPUStatusShowAcpiTemp = 1`

  Show ACPI temperature in CPU status tool tip.

- `CPUStatusShowAcpiTempInGraph = 0`

  Show ACPI temperature in CPU graph.

- `AcpiIgnoreBatteries =`
  List of battery names ignore.

- `CPUStatusShowCpuFreq = 1`

  Show CPU frequency in CPU status tool tip.

- `TaskBarShowMEMStatus = 1`

  Show memory usage status on task bar (Linux only).

- `TaskBarShowNetStatus = 1`

  Show network status on task bar (Linux only).

- `NetworkStatusDevice = "[ew]*"`
  List of network devices to be displayed in tray, space separated. Shell wildcard patterns can also be used.

- `TaskBarShowCollapseButton = 0`

  Show a button to collapse the taskbar.

- `TaskBarDoubleHeight = 0`

  Double height task bar

- `TaskBarWorkspacesLeft = 1`

  Place workspace pager on left, not right.

- `TaskBarWorkspacesTop = 0`

  Place workspace pager on top row when using dual-height taskbar.

- `PagerShowPreview = 1`

  Show a mini desktop preview on each workspace button. By pressing the middle mouse button the 'window list' is shown. The right button activates the 'window list menu'. By using the scroll wheel over the 'workspace list' one can quickly cycle over all workspaces.

- `PagerShowWindowIcons = 1`

  Draw window icons inside large enough preview windows on pager (if PagerShowPreview=1).

- `PagerShowMinimized = 1`

  Draw even minimized windows as unfilled rectangles (if PagerShowPreview=1).

- `PagerShowBorders = 1`

  Draw border around workspace buttons (if PagerShowPreview=1).

- `PagerShowNumbers = 1`

  Show number of workspace on workspace button (if PagerShowPreview=1).

- `TaskBarLaunchOnSingleClick = 1`

  Execute taskbar applet commands (like MailCommand, ClockCommand, ...) on single click.

- `EnableAddressBar = 1`

  Enable address bar functionality in taskbar.

- `ShowAddressBar = 1`

  Show address bar in task bar.

- `TimeFormat = "%X"`

  format for the taskbar clock (time) (see strftime(3) manpage).

- `TimeFormatAlt = ""`

  Alternate Clock Time format (e.g. for blinking effects).

- `DateFormat = "%c"`

  format for the taskbar clock tooltip (date+time) (see strftime(3) manpage).

- `TaskBarCPUSamples = 20`

  Width of CPU Monitor.

- `TaskBarMEMSamples = 20`

  Width of Memory Monitor.

- `TaskBarNetSamples = 20`

  Width of Net Monitor.

- `TaskbarButtonWidthDivisor = 3`

  Default number of tasks in taskbar.

- `TaskBarWidthPercentage = 100`

  Task bar width as percentage of the screen width.

- `TaskBarJustify = "left"`

  Taskbar justify left, right or center.

- `TaskBarApmGraphWidth = 10`

  Width of APM Monitor.

- `TaskBarGraphHeight = 20`

  Height of taskbar monitoring applets.

- `XineramaPrimaryScreen = 0`

  Primary screen for xinerama (taskbar, ...).

Mailbox Monitoring (updated 2018-03-04)
---------------------------------------

- `MailCheckDelay = 30`

  Delay between new-mail checks. (seconds).

- `MailBoxPath = ""`

This may contain a list of mailbox specifications. Mailboxes are separated by a space. If `TaskBarShowMailboxStatus` is enabled then IceWM will monitor each mailbox for status changes each `MailCheckDelay` seconds. For each mailbox IceWM will show an icon on the taskbar. The icon shows if there is mail, if there is unread mail, or if there is new mail. Hovering the mouse pointer over an icon shows the number of messages in this mailbox and also the number of unread mails. A mailbox can be the path to a file in conventional *mbox* format. If the path points to a directory then *Maildir* format is assumed. Remote mail boxes are specified by an URL using the Common Internet Scheme Syntax (RFC 1738):

    scheme://user:password@server[:port][/path]


Supported schemes are `pop3`, `pop3s`, `imap`, `imaps` and `file`. The `pop3s` and `imaps` schemes depend on the presence of the `openssl` command for `TLS/SSL` encryption. This is also the case if `port` is either `993` for imap or `995` for pop3. When the scheme is omitted then `file` is assumed. IMAP subfolders can be given by the path component. Reserved characters like *slash*, *at* and *colon* can be specified using escape sequences with a hexadecimal encoding like `%2f` for the slash or `%40` for the at sign. For example:

    file:///var/spool/mail/captnmark
    file:///home/captnmark/Maildir/
    pop3://markus:%2f%40%3a@maol.ch/
    pop3s://markus:password@pop.gmail.com/
    imap://mathias@localhost/INBOX.Maillisten.icewm-user
    imaps://mathias:password@imap.gmail.com/INBOX


To help solve network protocol errors for pop3 and imap set the environment variable `ICEWM_MAILCHECK_TRACE`. IceWM will then log communication details for POP3 and IMAP mailboxes. Just set `export ICEWM_MAILCHECK_TRACE=1` before executing icewm, or set this in the `env` configuration file.


Note that for IceWM to access Gmail you must first configure your Gmail account to enable POP3 or IMAP access. To allow non-Gmail applications like IceWM to use it see the Gmail help site for "Let less secure apps use your account". Also set secure file permissions on your IceWM preferences file and the directory which contains it. It is unwise to store a password on file ever. Consider a wallet extension for IceWM. The following Perl snippet demonstrates how to hex encode a password like `!p@a%s&s~`:

    $ perl -e 'foreach(split("", $ARGV[0])) { printf "%%%02x", ord($_); }; print "\n";' '!p@a%s&s~'
    %21%40%23%24%25%5e%26%2a%7e

- `NewMailCommand =`

  The command to be run when new mail arrives. It is executed by `/bin/sh -c`.
  The following environment variables will be set:

  * `ICEWM_MAILBOX` mailbox index number of `MailBoxPath` starting from 1.
  * `ICEWM_COUNT` gives the total number of messages in this mailbox.
  * `ICEWM_UNREAD` gives the number of unread messages in this mailbox.

Menus
-----

- `AutoReloadMenus = 1`

  Reload menu files automatically if set to 1.

- `ShowProgramsMenu = 0`

  Show programs submenu.

- `ShowSettingsMenu = 1`

  Show settings submenu.

- `ShowFocusModeMenu = 1`

  Show focus mode submenu.

- `ShowThemesMenu = 1`

  Show themes submenu.

- `ShowLogoutMenu = 1`

  Show logout menu.

- `ShowHelp = 1`

  Show the help menu item.

- `ShowLogoutSubMenu = 1`

  Show logout submenu.

- `ShowAbout = 1`

  Show the about menu item.

- `ShowRun = 1`

  Show the run menu item.

- `ShowWindowList = 1`

  Show the window menu item.

- `MenuMaximalWidth = 0`

  Maximal width of popup menus, 2/3 of the screen's width if set to zero.

- `NestedThemeMenuMinNumber = 25`

  Minimal number of themes after which the Themes menu becomes nested (0=disabled).

Timings
-------

- `DelayFuzziness = 10`

  Percentage of delay/timeout fuzziness to allow for merging of timer timeouts.

- `ClickMotionDistance = 5`

  Movement before click is interpreted as drag.

- `ClickMotionDelay = 200`

  Delay before click gets interpreted as drag.

- `MultiClickTime = 400`

  Time (ms) to recognize for double click.

- `MenuActivateDelay = 40`

  Delay before activating menu items.

- `SubmenuMenuActivateDelay = 300`

  Delay before activating menu submenus.

- `ToolTipDelay = 5000`

  Time before showing the tooltip.

- `ToolTipTime = 60000`

  Time before tooltip window is hidden (0 means never).

- `AutoHideDelay = 300`

  Time to auto hide taskbar (must enable first with TaskBarAutoHide).

- `AutoShowDelay = 500`

  Delay before task bar is shown.

- `AutoRaiseDelay = 400`

  Time to auto raise (must enable first with AutoRaise).

- `PointerFocusDelay = 200`

  Delay for pointer focus switching.

- `EdgeSwitchDelay = 600`

  Screen edge workspace switching delay.

- `ScrollBarStartDelay = 500`

  Initial scroll bar autoscroll delay

- `ScrollBarDelay = 30`

  Scroll bar autoscroll delay

- `AutoScrollStartDelay = 500`

  Auto scroll start delay

- `AutoScrollDelay = 60`

  Auto scroll delay

- `WorkspaceStatusTime = 2500`

  Time before workspace status window is hidden.

- `TaskBarCPUDelay = 500`

  Delay between CPU Monitor samples in ms.

- `TaskBarMEMDelay = 500`

  Delay between Memory Monitor samples in ms.

- `TaskBarNetDelay = 500`

  Delay between Net Monitor samples in ms.

- `FocusRequestFlashTime = 0`

  Number of seconds the taskbar app will blink when requesting focus (0 = forever).

- `FocusRequestFlashInterval = 250`

  Taskbar blink interval (ms) when requesting focus (0 = blinking disabled).

- `BatteryPollingPeriod = 10`

  Delay between power status updates (seconds).

Buttons and Keys
----------------

- `UseRootButtons = 255`

  Bitmask of root window button click to use in window manager.

- `ButtonRaiseMask = 1`

  Bitmask of buttons that raise the window when pressed.

- `DesktopWinMenuButton = 0`

  Desktop mouse-button click to show the window list menu.

- `DesktopWinListButton = 2`

  Desktop mouse-button click to show the window list.

- `DesktopMenuButton = 3`

  Desktop mouse-button click to show the root menu.

- `TitleBarMaximizeButton = 1`

  TitleBar mouse-button double click to maximize the window.

- `TitleBarRollupButton = 2`

  TitleBar mouse-button double click to rollup the window.

- `RolloverButtonsSupported = 0`

  Does it support the 'O' title bar button images (for mouse rollover)

Workspaces
----------

- WorkspaceNames

  List of workspace names, for example:

    WorkspaceNames=" 1 ", " 2 ", " 3 ", " 4 "

Paths
-----

- LibPath

  Path to the icewm/lib directory.

- IconPath

  Path to the icon directory. Multiple paths can be given using the colon as a separator.

Programs
--------

- ClockCommand

  program to run when the clock is double clicked.

- MailCommand

  program to run when mailbox icon is double clicked.

- LockCommand

  program to run to lock the screen.

- RunCommand

  program to run when **Run** is selected from the start menu.

Window Menus
------------

WinMenuItems
Items to show in the window menus, possible values are:

- `  a=rAise`


- `  c=Close`


- `  f=Fullscreen`


- `  h=Hide`


- `  i=trayIcon`


- `  k=Kill`


- `  l=Lower`


- `  m=Move`


- `  n=miNimize`


- `  r=Restore`


- `  s=Size`


- `  t=moveTo`


- `  u=rollUp`


- `  w=WindowsList`


- `  x=maXimize`


- `  y=laYer`

  Examples:


    WinMenuItems=rmsnxfhualyticw   #Default menu
    WinMenuItems=rmsnxfhualytickw  #Menu with all possible options
    WinMenuItems=rmsnxc            #MS-Windows menu

[Prev](icewm-9.html) [Top](icewm-toc.html) [Next](icewm-11.html)
