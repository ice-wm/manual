---
title: Command Line Options - IceWM Manual
---

[Prev](icewm-17.html) [Top](icewm-toc.html) [Next](icewm-19.html)

Command Line Options
====================

`icewm` supports the following options:

    -d, --display=NAME
    NAME of the X server to use.

    --client-id=ID
    Client id to use when contacting session manager.

    --sync
    Synchronize X11 commands.

    -c, --config=FILE
    Load preferences from FILE.

    -t, --theme=FILE
    Load theme from FILE.

    --postpreferences
    Print preferences after all processing.

    -V, --version
    Prints version information and exits.

    -h, --help
    Prints this usage screen and exits.

    --replace
    Replace an existing window manager.

    -r, --restart
    Tell the running icewm to restart itself.

    --configured
    Print the compile time configuration.

    --directories
    Print the configuration directories.

    -l, --list-themes
    Print a list of all available themes.

The restart option can be used to reload the IceWM configuration after modifications. It is the preferred way to restart IceWM from the command line or in scripts. To load a different theme from the command line, combine this with the `--theme=NAME` option like:

    icewm -r -t CrystalBlue

The theme name will then be saved to the 'theme' configuration file, before restarting IceWM.

[Prev](icewm-17.html) [Top](icewm-toc.html) [Next](icewm-19.html)
