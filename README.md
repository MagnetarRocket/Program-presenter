## Program-presenter

A OS/2 1.2 + 1.3, Win 3.X - like x11 window manager. Has some features from "Amish System Utilities" integrated as basic functionality.

![progman screenshot](https://jcs.org/images/progman-20200810.png)

### License

MIT

### Compiling

Run `make` to compile, and `make install` to install to `/usr/local` by
default.

To uninstall, run `make uninstall`.

### Features

- Window minimizing, drawing icons and labels on the root/desktop
- Window maximizing by double-clicking on a window titlebar, and full-screen
  support (via `_NET_WM_STATE_FULLSCREEN`)
- Window shading by right-clicking on a window titlebar
- Window moving by holding down `Alt` (configurable) and clicking anywhere on a
  window
- Built-in menu acessed via the right mouse-button by default, menu can be ajusted by the user.
- Window menus, can use window hints a-la the motif wm.
- Built-in keyboard binding support by adding items to the `[keyboard]`
  section of `~/.config/progman/progman.ini` such as `Win+L = exec xlock`
- Built-in mouse button binding on the desktop by adding items to the
  `[desktop]` section of `~/.config/progman/progman.ini` such as
  `Mouse3 = exec xterm`, with right-click setup by default to show a
  configurable launcher menu containing programs listed in the `[launcher]`
  section of `progman.ini`
- Virtual desktops with keyboard shortcuts for switching between them bound
  to `Alt+1` through `Alt+0` by default, and using the mouse wheel on the
  desktop to scroll through virtual desktops
- Window cycling with `Alt+Tab` and `Shift+Alt+Tab`
- [Theme support](https://github.com/jcs/progman/tree/master/themes)
- Optional HiDPI scaling support to magnify icons and buttons
