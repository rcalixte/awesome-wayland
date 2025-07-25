<h1 align="center">
  <samp style="color: #ffffff; background-color: #ffbc00;">Awesome Wayland</samp>

[![Link Check](https://github.com/rcalixte/awesome-wayland/actions/workflows/link_check.yml/badge.svg?branch=master)](https://github.com/rcalixte/awesome-wayland/actions/workflows/link_check.yml)
</h1>

A curated list of [Wayland](https://gitlab.freedesktop.org/wayland/wayland) resources. Please investigate these projects on your own before fully committing to them!

This repository is a hard fork of [natpen/awesome-wayland](https://github.com/natpen/awesome-wayland) since it was archived on Oct. 17, 2023.

There are no current plans to apply to the [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) project for inclusion.

> [!NOTE]
> If you want to contribute, please read [this](https://github.com/rcalixte/awesome-wayland/blob/master/.github/CONTRIBUTING.md).

SCOPE
-----

> [!IMPORTANT]
> The scope of this repository aims to capture applications, libraries, etc. that are **designed** to support the Wayland ecosystem. This does not include existing applications that have implemented support for Wayland. That list is being maintained at [mpsq/arewewaylandyet](https://github.com/mpsq/arewewaylandyet) which is the repository for [arewewaylandyet.com](https://arewewaylandyet.com). An updated list is also available at [gianklug/wearewaylandnow](https://github.com/gianklug/wearewaylandnow) which is the repository for [wearewaylandnow.com](https://wearewaylandnow.com).

TABLE OF CONTENTS
-----------------

- [SCOPE](#scope)
- [TABLE OF CONTENTS](#table-of-contents)
- [BINDINGS](#bindings)
- [BREAK NOTIFIERS](#break-notifiers)
- [BRIGHTNESS CONTROL](#brightness-control)
- [CLIPBOARD MANAGERS](#clipboard-managers)
- [COMPOSITORS](#compositors)
- [DISPLAY CONFIGURATION](#display-configuration)
- [EMULATION](#emulation)
- [IMAGE VIEWING](#image-viewing)
- [LAUNCHERS](#launchers)
- [LIBRARIES](#libraries)
- [NOTIFICATIONS](#notifications)
- [ON-SCREEN KEYBOARDS](#on-screen-keyboards)
- [REFERENCE APPLICATIONS](#reference-applications)
- [SCREEN LOCKING](#screen-locking)
- [SCREENCASTS](#screencasts)
- [SCREENSHOTS](#screenshots)
- [SESSION MANAGEMENT](#session-management)
- [THEMING](#theming)
- [TOOLS](#tools)
- [WALLPAPER](#wallpaper)
- [WIDGETS (BARS, PANELS, ETC.)](#widgets-bars-panels-etc)

BINDINGS
--------

These are language-specific bindings for use with Wayland development.

- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [pywayland](https://github.com/flacjacket/pywayland) - A wrapper to the libwayland library

BREAK NOTIFIERS
---------------

- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Ianny](https://github.com/zefr0x/ianny) - Periodically informs user to take breaks by keeping track of usage patterns

BRIGHTNESS CONTROL
------------------

No Wayland-specific requirements, so you can use your Xorg solution of choice to control screen brightness, like [brightnessctl](https://github.com/Hummer12007/brightnessctl), [brillo](https://gitlab.com/cameronnemo/brillo), or just directly manipulate `/sys/class/backlight`.

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Clight](https://github.com/FedeDP/Clight) - Day/night gamma adjustments for Wayland compositors supporting `wlr-gamma-control-unstable-v1`; automatic screen backlight calibration to match ambient brightness using either webcam or ambient light sensor devices; screen dimming
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Gammastep](https://gitlab.com/chinstrap/gammastep) - A day/night gamma modifier that adjusts the color temperature of the screen
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Luminance](https://github.com/sidevesh/Luminance) - A simple GTK application to control brightness of displays including external displays supporting DDC/CI
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wl-gammactl](https://github.com/mischw/wl-gammactl) - A GTK application to set contrast, brightness, and gamma using the `wlr-gamma-control` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlsunset](https://git.sr.ht/~kennylevinsen/wlsunset) - A day/night gamma adjustments for Wayland compositors supporting `wlr-gamma-control-unstable-v1` and `xdg-output-unstable-v1` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wluma](https://github.com/maximbaz/wluma) - A tool for wlroots-based compositors that automatically adjust screen brightness based on screen contents and ambient light
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [yabd](https://github.com/tbrugere/yabd) - A simple brightness daemon compatible with Wayland compositors

CLIPBOARD MANAGERS
------------------

- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [clapboard](https://github.com/bjesus/clapboard) - A clipboard manager with support for images and saved entries
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [cliphist](https://github.com/sentriz/cliphist) - A clipboard history manager for Wayland
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [clipman](https://github.com/chmouel/clipman) - A simple clipboard manager implementing the `wlr-data-control-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [gemclip](https://codeberg.org/novenary/gemclip) - A simple clipboard utility for Wayland implementing the `wlr-data-control-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wayclip](https://github.com/noocsharp/wayclip) - A Wayland clipboard utility implementing the `wlr-data-control-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - Command-line copy/paste utilities for Wayland
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlsnarf](https://codeberg.org/notchoc/wlsnarf) - A highly scriptable clipboard tool for wlroots-based compositors implementing the `wlr-data-control-unstable-v1` protocol; includes a filesystem-based clipboard manager daemon with persistence

COMPOSITORS
-----------

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Cagebreak](https://github.com/project-repo/cagebreak) - A Wayland tiling compositor inspired by Ratpoison
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Cage](https://github.com/cage-kiosk/cage) - A Wayland compositor that runs a single application in maximized mode, particularly suitable for kiosk applications
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [croissant](https://codeberg.org/vyivel/croissant) - A wlroots-based stacking Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [CwC](https://github.com/Cudiph/cwcwm) - A highly configurable wlroots-based tiling window manager, inspired by AwesomeWM
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [dwl](https://codeberg.org/dwl/dwl) - A wlroots-based rewrite of DWM for Wayland
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [foxwhale](https://github.com/malcolmstill/foxwhale) - A tiling Wayland compositor based on wlroots
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [Gabbia](https://github.com/heuer/gabbia) - A Wayland compositor inspired by Cage that runs a single application in maximized mode, particularly suitable for kiosk applications
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [gamescope](https://github.com/ValveSoftware/gamescope) - A wlroots-based Wayland compositor designed for SteamOS
- ![Nim](https://img.shields.io/badge/nim-%23171921.svg?style=plastic&logo=nim&logoColor=ffe953) [gogh](https://github.com/xTrayambak/gogh) - A lightweight Wayland compositor using Louvre
- ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=plastic&logo=javascript&logoColor=%23f7df1e) [Greenfield](https://github.com/udevbe/greenfield) - An HTML5 Wayland compositor that runs directly in the browser
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [hikari](https://hub.darcs.net/raichoo/hikari) - A hybrid stacking/tiling Wayland compositor based on wlroots
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Hopalong](https://github.com/iridescent-desktop/hopalong) - A simple Wayland compositor with a feature set comparable to XFWM
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Hyprland](https://github.com/hyprwm/Hyprland) - A dynamic tiling Wayland compositor that doesn't sacrifice on its looks
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [japokwm](https://github.com/werererer/japokwm) - A wlroots-based dynamic tiling Wayland compositor based around creating layouts
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Jay](https://github.com/mahkoh/jay) - A tiling Wayland compositor inspired by i3wm
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [kiwmi](https://github.com/buffet/kiwmi) - A fully programmable Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [labwc](https://github.com/labwc/labwc) - A wlroots-based stacking compositor for Wayland, inspired by openbox
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [LaikaWM](https://github.com/ianmartinez/laikawm) - A lightweight compositor for Wayland inspired by IceWM and Fluxbox
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Liri Shell](https://github.com/lirios/shell) - A convergent shell for desktops, phones, and tablets
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Magpie v1](https://github.com/buddiesofbudgie/magpie/tree/v1) - A wlroots-based Wayland compositor designed for the Budgie desktop environment
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff)&nbsp;![Lisp](https://img.shields.io/badge/lisp-%23000.svg?style=plastic&logo=lisp&logoColor=fff) [mahogany](https://github.com/stumpwm/mahogany) - A StumpWM-like Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [maomaowm](https://github.com/DreamMaoMao/maomaowm) - A dwl-inspired Wayland compositor with lightweight animations and customizable layouts
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [miracle-wm](https://github.com/miracle-wm-org/miracle-wm) - A Mir-based tiling Wayland compositor
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Miriway](https://github.com/Miriway/Miriway) - A Mir-based Wayland compositor
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [newm-atha](https://git.sr.ht/~atha/newm-atha) - A Wayland compositor written with laptops and touchpads in mind
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [niri](https://github.com/YaLTeR/niri) - A scrollable tiling Wayland compositor
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [Nyctal](https://github.com/s-rah/nyctal) - A tiny, minimal-dependency Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [phoc](https://gitlab.gnome.org/World/Phosh/phoc) - A wlroots-based Wayland compositor mostly used on mobile phones
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [pinnacle](https://github.com/pinnacle-comp/pinnacle) - A wlroots-based Wayland compositor inspired by AwesomeWM
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [river](https://codeberg.org/river/river) - A dynamic tiling Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [stagen](https://github.com/lidgnulinux/stagen) - An experimental wlroots-based Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [SwayFX](https://github.com/WillPower3309/swayfx) - Sway, but with eye candy
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [sway](https://github.com/swaywm/sway) - An i3-compatible Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [tinybox](https://github.com/icedman/tinybox) - A window manager based on tinywl inspired by Blackbox, Fluxbox, and Openbox
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [tinywl+](https://github.com/keshto/tinywl_plus) - A stacking Wayland compositor based on tinywl and a great starting place for compositor development
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [turtile](https://github.com/migueldeoleiros/turtile) - A simple and customizable wlroots-based tiling compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [velox](https://github.com/michaelforney/velox) - A simple window manager based on swc, inspired by dwm and xmonad
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Vivarium](https://github.com/inclement/vivarium) - A dynamic tiling Wayland compositor using wlroots, with desktop semantics inspired by xmonad
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [volare](https://codeberg.org/raboof/volare) - A tiling, tabbed Wayland compositor
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Waybox](https://github.com/wizbright/waybox) - An openbox clone on Wayland
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Wayfire](https://github.com/WayfireWM/wayfire) - A 3D wlroots-based Wayland compositor inspired by Compiz
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wayward](https://github.com/varmd/wayward) - A lightweight desktop shell compatible with Weston
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Weston](https://gitlab.freedesktop.org/wayland/weston/) - A Wayland compositor designed for correctness, reliability, predictability, and performance
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlmaker](https://github.com/phkaeser/wlmaker) - A Wayland compositor inspired by Window Maker
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Woodland](https://github.com/DiogenesN/woodland) - A minimal and lightweight wlroots-based stacking compositor, inspired by Wayfire and TinyWL

DISPLAY CONFIGURATION
---------------------

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Kanshi](https://gitlab.freedesktop.org/emersion/kanshi) - A dynamic display configuration tool for Wayland similar to autorandr, usable on Wayland compositors supporting the `wlr-output-management` protocol
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [nwg-displays](https://github.com/nwg-piotr/nwg-displays) - An output management utility for sway and Hyprland, inspired by wdisplays and wlay
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [shikane](https://gitlab.com/w0lff/shikane) - A wlroots-based dynamic output configuration tool similar to autorandr, usable on Wayland compositors supporting the `wlr-output-management` protocol
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [Wallutils](https://github.com/xyproto/wallutils) - A set of utilities to handle monitors, resolutions, wallpapers, and timed wallpapers
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [wayland-displays](https://github.com/heyzec/wayland-displays) - A GUI and CLI tool for managing display outputs on wlroots-based Wayland compositors implementing the `wlr-output-management-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wayout](https://git.sr.ht/~shinyzenith/wayout) - A simple output management tool for wlroots-based compositors implementing `wlr-output-management-unstable-v1`
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wdisplays](https://github.com/artizirk/wdisplays) - A GUI application for configuring displays in wlroots-based compositors implementing the `wlr-output-management-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlay](https://github.com/atx/wlay) - Graphical output management for Wayland
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlr-randr](https://gitlab.freedesktop.org/emersion/wlr-randr) - A utility to manage outputs of wlroots-based Wayland compositors, inspired by xrandr

EMULATION
---------

- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [Waydroid](https://github.com/waydroid/waydroid) - A container-based approach to boot a full Android system on GNU/Linux

IMAGE VIEWING
-------------

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Swayimg](https://github.com/artemsen/swayimg) - An image viewer for Sway/Wayland

LAUNCHERS
---------

- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Anyrun](https://github.com/anyrun-org/anyrun) - A GTK-based Wayland-native launcher, customizable via CSS
- ![Nim](https://img.shields.io/badge/nim-%23171921.svg?style=plastic&logo=nim&logoColor=ffe953) [basket](https://github.com/xTrayambak/basket) - A minimal application launcher for Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [bemenu](https://github.com/Cloudef/bemenu) - A dynamic menu library and client program inspired by dmenu
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [diowapplauncher](https://github.com/DiogenesN/diowapplauncher) - A simple application launcher for Wayland compositors implementing the `xdg-shell` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [diowmenu](https://github.com/DiogenesN/diowmenu) - A simple quick launch menu for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [dmenu-wayland](https://github.com/nyyManni/dmenu-wayland) - A wlroots-based dynamic menu for Wayland
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [emenu](https://codeberg.org/fbushstone/emenu) - An efficient menu for wlroots-based Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [fuzzel](https://codeberg.org/dnkl/fuzzel) - An application launcher for wlroots-based Wayland compositors, similar to rofi's `drun` mode
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [gmenu](https://codeberg.org/tslocum/gmenu) - A desktop application launcher
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [kickoff](https://github.com/j0ru/kickoff) - A wlroots-based application launcher
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [LavaLauncher](https://git.sr.ht/~leon_plickat/lavalauncher) - A simple launcher panel for Wayland desktops
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Mauncher](https://github.com/mortie/mauncher) - A GTK-based alternative to dmenu for Wayland which supports display scaling
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [mew](https://codeberg.org/sewn/mew) - A dmenu-like dynamic menu for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [mounch](https://github.com/chmouel/mounch) - A simple wofi/rofi launcher configured via YAML
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [nwg-launchers](https://github.com/nwg-piotr/nwg-launchers) - A GTK-based application grid launcher, button bar, and dmenu for Sway with a best effort for other Wayland environments
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [rofi](https://github.com/lbonn/rofi) - A fork of rofi with Wayland support
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [sirula](https://github.com/DorianRudolph/sirula) - A simple application launcher for Wayland
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [sysmenu](https://github.com/System64fumo/sysmenu) - A simple program launcher for wlroots-based Wayland compositors, implementing the `gtk4-layer-shell` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [tofi](https://github.com/philj56/tofi) - A dynamic menu replacement for dmenu or rofi for wlroots-based Wayland compositors
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [walker](https://github.com/abenz1267/walker) - A GTK-based Wayland-native application runner
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [waylauncher](https://github.com/tomipkoskinen/waylauncher) - A GTK-based application launcher implementing the `gtk4-layer-shell` protocol
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [waypiedock](https://gitlab.com/Arnaudv6/waypiedock) - A launcher dock, in the shape of a pie, under the mouse
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wldash](https://github.com/kennylevinsen/wldash) - A dashboard, launcher, or control panel for Wayland, using the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wmenu](https://codeberg.org/adnano/wmenu) - A dynamic menu for Sway and wlroots-based compositors inspired by dmenu
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [yofi](https://github.com/l4l/yofi) - A minimalistic menu for Wayland-based compositors

LIBRARIES
---------

- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [client-toolkit](https://github.com/Smithay/client-toolkit) - A toolkit for writing Wayland clients in Rust
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [glace](https://github.com/Fabric-Development/glace) - A GTK-based library that aids in the management of Wayland clients such as docks and desktop widgets
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [gtk4-layer-shell](https://github.com/wmww/gtk4-layer-shell) - A library to create panels and other desktop components for Wayland using GTK 4 and the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [gtk-layer-shell](https://github.com/wmww/gtk-layer-shell) - A library to create panels and other desktop components for Wayland using GTK 3 and the `wlr-layer-shell-unstable-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [layer-shell-qt](https://github.com/KDE/layer-shell-qt) - A Qt-based library to allow applications to use the `wlr-layer-shell-unstable-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Louvre](https://github.com/CuarzoSoftware/Louvre) - A library designed for building Wayland compositors in C++
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Mir](https://github.com/canonical/mir) - A set of libraries for building Wayland-based shells
- ![OCaml](https://img.shields.io/badge/ocaml-%23ededed.svg?style=plastic&logo=ocaml&logoColor=ec670f) [ocaml-wayland](https://github.com/talex5/ocaml-wayland) - An implementation of the Wayland protocol in OCaml
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [smithay](https://github.com/Smithay/smithay) - A compositor library for Wayland
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [swc](https://github.com/michaelforney/swc) - A small Wayland compositor implemented as a library
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Swingby](https://github.com/aspschn/swingby) - A small GUI library for Wayland client programming
- ![Dart](https://img.shields.io/badge/dart-29b6f6?style=plastic&logo=dart&logoColor=01579b) [wayland-dart](https://github.com/kingwill101/wayland-dart) - A Dart implementation of the Wayland client protocols
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [way-z](https://github.com/psnszsn/way-z) - A client library and widget toolkit for wlroots-based Wayland applications written in Zig
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wld](https://github.com/michaelforney/wld) - A drawing library that targets Wayland
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlroots](https://gitlab.freedesktop.org/wlroots/wlroots/) - Pluggable, composable, and unopinionated modules for building a Wayland compositor
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Wrapland](https://github.com/winft/wrapland) - A Qt-based wrapper library for the libwayland client and server APIs
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [zig-wlroots](https://codeberg.org/ifreund/zig-wlroots) - Bindings to wlroots for Zig for developing Wayland compositors and clients

NOTIFICATIONS
-------------

- ![Vala](https://img.shields.io/badge/vala-%237b6ca3.svg?style=plastic&logo=vala&logoColor=fff) [Avizo](https://github.com/heyjuvi/avizo) - A simple notification daemon, mainly intended to be used for multimedia keys
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [dunst](https://github.com/dunst-project/dunst) - A highly configurable and lightweight notification daemon
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [fnott](https://codeberg.org/dnkl/fnott) - A keyboard-driven and lightweight notification daemon for wlroots-based Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [luft](https://codeberg.org/marendowski/luft) - A lightweight notification daemon for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [mako](https://github.com/emersion/mako) - A lightweight notification daemon for Wayland implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Vala](https://img.shields.io/badge/vala-%237b6ca3.svg?style=plastic&logo=vala&logoColor=fff) [SwayNotificationCenter](https://github.com/ErikReider/SwayNotificationCenter) - A simple notification daemon with a GTK GUI for notifications and the control center implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [SwayOSD](https://github.com/ErikReider/SwayOSD) - A GTK-based OSD window for common actions like volume and Caps Lock

ON-SCREEN KEYBOARDS
-------------------

- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [wf-osk](https://github.com/WayfireWM/wf-osk) - A very, very basic on-screen keyboard using gtkmm and the `virtual-keyboard-unstable-v1` and `wlr-layer-shell-unstable-v1` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wkeys](https://github.com/ptazithos/wkeys) - An on-screen keyboard featuring a configurable layout and style for Wayland compositors supporting the `gtk4-layer-shell` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wshowkeys](https://git.sr.ht/~sircmpwn/wshowkeys) - Displays keypresses on screen on Wayland compositors supporting the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wvkbd](https://github.com/jjsullivan5196/wvkbd) - An on-screen keyboard for wlroots-based compositors

REFERENCE APPLICATIONS
----------------------

These are mainly for developers looking for example implementations.

- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [go-wayland](https://github.com/MatthiasKunnen/go-wayland) - A basic implementation of the Wayland protocol
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [vkwayland](https://github.com/kdchambers/vkwayland) - A reference application for Vulkan and Wayland
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [wayland-py](https://github.com/aslpavel/wayland-py) - A pure Python implementation of a Wayland client
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [zig-wayland](https://codeberg.org/ifreund/zig-wayland) - A basic implementation of the Wayland protocol for developing Wayland compositors and clients, including examples

SCREEN LOCKING
--------------

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Anvilock](https://github.com/muvilon/anvilock) - A simple screen-locker for Wayland compositors that support the `ext-session-lock-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [chayang](https://git.sr.ht/~emersion/chayang) - A screen dimmer that can be used to implement a grace period before locking the session
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [cthulock](https://github.com/FriederHannenheim/cthulock) - A Slint-based customizable screen-locker for Wayland compositors implementing the `ext-session-lock-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [gtklock](https://github.com/jovanlanik/gtklock) - A GTK-based lockscreen for wlroots-based Wayland compositors using the `wlr-layer-shell-unstable-v1` and `wlr-input-inhibitor` Wayland protocols
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [hypridle](https://github.com/hyprwm/hypridle) - A wlroots-based idle management daemon implementing the `ext-idle-notify-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [hyprlock](https://github.com/hyprwm/hyprlock) - A multi-threaded and GPU-accelerated wlroots-based screen locking utility implementing the `ext-session-lock-v1` and `wlr-screencopy-unstable-v1` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Shaderlock](https://github.com/RobinMcCorkell/shaderlock) - A wlroots-based screen-locker for Wayland utilizing GPU shaders
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [swayidle](https://github.com/swaywm/swayidle) - An idle management daemon for Wayland which implements the `ext-idle-notify-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [swaylock-effects](https://github.com/mortie/swaylock-effects) - A fork of swaylock which adds, built-in screenshots, image manipulation, and various other effects like blurring
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [swaylock](https://github.com/swaywm/swaylock) - A screen locking utility for Wayland which implements the `ext-idle-notify-v1` protocol protocol
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [waylock](https://codeberg.org/ifreund/waylock) - A small screen-locker for Wayland compositors implementing the `ext-session-lock-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlock](https://codeberg.org/sewn/wlock) - A simple screen-locker for Wayland compositors that support the `ext-session-lock-v1` protocol

SCREENCASTS
-----------

- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Kooha](https://github.com/SeaDve/Kooha) - Minimalistic screen recorder for Wayland sessions implementing the `org.freedesktop.impl.portal.ScreenCast` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [ssr-wlroots](https://github.com/foxcpp/ssr-wlroots) - A fork of SimpleScreenRecorder with support for wlroots-based compositors (more specifically, those that support `wlr-screencopy-unstable-v1` and `xdg-output-unstable-v1`) - doesn't support recording area selection and has issues with multiple screens
- ![Vala](https://img.shields.io/badge/vala-%237b6ca3.svg?style=plastic&logo=vala&logoColor=fff) [wayfarer](https://github.com/stronnag/wayfarer) - A screen recorder for GNOME/Wayland/PipeWire implementing the `org.freedesktop.impl.portal.ScreenCast` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [wayrec](https://invent.kde.org/bharadwaj-raju/wayrec) - A simple screen recorder using the `org.freedesktop.impl.portal.ScreenCast` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [wf-recorder](https://github.com/ammen99/wf-recorder) - A utility program for screen recording of wlroots-based compositors (more specifically, those that support `wlr-screencopy-unstable-v1` and `xdg-output-unstable-v1`)
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wl-mirror](https://github.com/Ferdi265/wl-mirror) - A simple Wayland output mirror client
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlrobs](https://hg.sr.ht/~scoopta/wlrobs) - A plugin for OBS Studio that allows screen capture on wlroots-based Wayland compositors
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wl-screenrec](https://github.com/russelltg/wl-screenrec) - A screen recorder for wlroots-based Wayland compositors leveraging DMA-BUF and the DRM and implementing the `wlr-output-management-unstable-v1` and `wlr-screencopy-unstable-v1` protocols

SCREENSHOTS
-----------

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [dulcepan](https://codeberg.org/vyivel/dulcepan) - A screenshot tool for wlroots-based Wayland compositors, implementing the `wlr-layer-shell-unstable-v1` and `wlr-screencopy-unstable-v1` protocols
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [grim](https://gitlab.freedesktop.org/emersion/grim) - Grab images from a Wayland compositor
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [haruhishot](https://github.com/Decodetalkers/haruhishot) - A screenshot utility for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` and `wlr-screencopy-unstable-v1` protocols
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [samurai-select](https://github.com/Samudevv/samurai-select) - A screen selection tool for wlroots-based Wayland compositors implementing `wlr-layer-shell-unstable-v1`
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Satty](https://github.com/gabm/Satty) - A screenshot annotation tool inspired by Swappy and Flameshot
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [Seto](https://github.com/unixpariah/Seto) - A hardware-accelerated and keyboard-driven screen selection tool implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [shotman](https://git.sr.ht/~whynothugo/shotman) - A screenshot GUI for Wayland compositors implementing `wlr-layer-shell-unstable-v1`, `wlr-screencopy-unstable-v1`, and `single-pixel-buffer-v1` protocols
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [slurp](https://github.com/emersion/slurp) - Select a region in a Wayland compositor and print it to the standard output
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [swappy](https://github.com/jtheoof/swappy) - A Wayland-native snapshot editing tool, inspired by Snappy on macOS
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Taiga](https://hg.sr.ht/~scoopta/taiga) - An animated screenshot program for wlroots-based Wayland compositors
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Watershot](https://github.com/Kirottu/watershot) - A simple Wayland-native screenshot tool inspired by Flameshot
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Wayshot](https://git.sr.ht/~shinyzenith/wayshot) - A screenshot tool for wlroots-based compositors implementing `wlr-screencopy-unstable-v1`
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [waysip](https://github.com/waycrate/waysip) - An area selector for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Weye](https://github.com/Yakkhini/Weye) - A lightweight screenshot tool for sway users

SESSION MANAGEMENT
------------------

- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [nwg-bar](https://github.com/nwg-piotr/nwg-bar) - A Wayland-based logout menu implementing the `gtk3-layer-shell` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [SwayAudioIdleInhibit](https://github.com/ErikReider/SwayAudioIdleInhibit) - Prevents swayidle from sleeping while any application is outputting or receiving audio, implementing the `idle-inhibit-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wleave](https://github.com/AMNatty/wleave) - A Wayland-based logout menu implementing the `gtk3-layer-shell` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlogout](https://github.com/ArtsyMacaw/wlogout) - A Wayland-based logout menu

THEMING
-------

- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [nwg-look](https://github.com/nwg-piotr/nwg-look) - A GTK 3 settings editor designed to work properly in a wlroots-based environment

TOOLS
-----

- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [clipcell](https://github.com/divadiahim/clipcell) - A clipboard manager with support for text and image preview for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [dd99 Wayland Library](https://github.com/Delta-dev-99/dd99_wayland) - A Wayland protocol scanner
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Door Knocker](https://codeberg.org/tytan652/door-knocker) - A simple tool to check the availability of XDG portals in a running session
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [hyprpicker](https://github.com/hyprwm/hyprpicker) - A wlroots-compatible Wayland color picker
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [lan-mouse](https://github.com/feschber/lan-mouse) - A mouse and keyboard sharing software
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [lswt](https://git.sr.ht/~leon_plickat/lswt) - List Wayland toplevels in both human readable and machine parsable formats via the `wlr-foreign-toplevel-management-unstable-v1` protocol
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [Meadhall](https://github.com/hkupty/meadhall) - A Wayland utilities daemon designed to centralize communication
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [scenefx](https://github.com/wlrfx/scenefx) - A drop-in replacement for the wlroots scene-graph API that allows Wayland compositors to render surfaces with eye-candy effects
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [sway-fader](https://github.com/mgnsk/sway-fader) - A tool that can be used to control transparency for focus and window events
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Vigiland](https://github.com/Jappie3/vigiland) - An application implementing the `idle-inhibit-unstable-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Waycheck](https://gitlab.freedesktop.org/serebit/waycheck) - A simple application that displays all of the Wayland protocols supported and unsupported by the running compositor
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [waycorner](https://github.com/AndreasBackx/waycorner) - Hot corners for wlroots-based Wayland compositors implementing the `xdg-output-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [waydapt](https://gitlab.freedesktop.org/jonleivent/waydapt) - A Wayland compositor protocol adapter that can proxy or filter communication between a compositor and one or more clients
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [wayland-debug](https://github.com/wmww/wayland-debug) - A command-line tool for debugging Wayland clients and servers
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [wayland-display-info](https://github.com/acrion/wayland-display-info) - A lightweight user daemon that monitors Wayland outputs via the `wlr-output-management-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [waylevel](https://git.sr.ht/~shinyzenith/waylevel) - A simple debugging tool which prints Wayland toplevels and other compositor specific information
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [waynergy](https://github.com/r-c-f/waynergy) - An implementation of a synergy client for Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [waypipe](https://gitlab.freedesktop.org/mstoeckl/waypipe) - A proxy for Wayland clients enabling application forwarding similar to `ssh -X`
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [wayprompt](https://git.sr.ht/~leon_plickat/wayprompt) - A multi-purpose prompt tool for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wayvnc](https://github.com/any1/wayvnc) - A VNC server for wlroots-based Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wev](https://git.sr.ht/~sircmpwn/wev) - A tool for debugging events on a Wayland window, analogous to the X11 tool `xev`
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [whisper-overlay](https://github.com/oddlama/whisper-overlay) - A tool providing speech-to-text functionality for Wayland compositors implementing `virtual-keyboard-unstable-v1` and `wlr-layer-shell-unstable-v1` protocols
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [wlcs](https://github.com/canonical/wlcs) - A protocol-conformance-verifying test suite usable by Wayland compositor implementors
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [wledges](https://github.com/fshaked/wledges) - A tool for managing screen edges on wlroots-based Wayland compositors implementing the `gtk4-layer-shell` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlinhibit](https://github.com/0x5a4/wlinhibit) - A simple idle inhibitor implementing the `idle-inhibit-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wl-kbptr](https://github.com/moverest/wl-kbptr) - A utility to help move the mouse pointer with the keyboard implementing the `wlr-layer-shell-unstable-v1` and `wlr-virtual-pointer-unstable-v1` protocols
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlopm](https://git.sr.ht/~leon_plickat/wlopm) - A Wayland output power management tool implementing the `wlr-output-power-management-unstable-v1` protocol
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [wlosd](https://github.com/fshaked/wlosd) - An on-screen display for Wayland compositors implementing the `gtk4-layer-shell` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlrctl](https://git.sr.ht/~brocellous/wlrctl) - A command-line utility for miscellaneous wlroots-based Wayland extensions, supporting the `wlr-foreign-toplevel-management-unstable-v1`, `virtual-keyboard-unstable-v1`, and `wlr-virtual-pointer-unstable-v1` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wlr-which-key](https://github.com/MaxVerevkin/wlr-which-key) - A keymap manager for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wtw](https://github.com/sewnie/wtw) - A simple text widget for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wtype](https://github.com/atx/wtype) - A Wayland tool that allows keyboard input simulation like [`xdotool`](https://github.com/jordansissel/xdotool)
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [xwayland-run](https://gitlab.freedesktop.org/ofourdan/xwayland-run) - A set of utilities revolving around running `Xwayland` and various Wayland compositors headless
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [ydotool](https://github.com/ReimuNotMoe/ydotool) - A generic Linux command-line automation tool

WALLPAPER
---------

- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [Azote](https://github.com/nwg-piotr/azote) - A GTK 3-based picture browser and background setter supporting all wlroots-based Wayland compositors
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [beanbag](https://codeberg.org/bwbuhse/beanbag) - A lightweight wallpaper application designed for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [glshell](https://github.com/Duckonaut/glshell) - A shader display implementing the `wlr-layer-shell-unstable-v1` protocol that can be used to create a simple overlay for a Wayland compositor, a status bar, or a wallpaper
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Hyprpaper](https://github.com/hyprwm/hyprpaper) - A wallpaper utility with the ability to dynamically change wallpapers supporting all wlroots-based compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [mpvpaper](https://github.com/GhostNaN/mpvpaper) - A video wallpaper program for wlroots-based Wayland compositors
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [rwpspread](https://github.com/0xk1f0/rwpspread) - A multi-monitor wallpaper utility spanning input wallpapers across all monitors, supporting Wayland compositors implementing `xdg-output-unstable-v1` with integrations for `wpaperd`, `swaybg`, `hyprpaper`, `swaylock`, and `hyprlock`
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [swaybg](https://github.com/swaywm/swaybg) - A wallpaper utility for Wayland compositors implementing the `wl_output` version 4 and `wlr-layer-shell-unstable-v1` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [swww](https://github.com/LGFae/swww) - An animated wallpaper daemon for Wayland, controlled at runtime and implementing the `wlr-layer-shell-unstable-v1` and `xdg-output-unstable-v1` protocols
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [Wallutils](https://github.com/xyproto/wallutils) - A set of utilities to manage monitors, resolutions, wallpapers and timed wallpapers
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [Waypaper](https://github.com/anufrievroman/waypaper) - A GUI frontend for swaybg/swww to switch wallpapers
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wbg](https://codeberg.org/dnkl/wbg) - A simple wallpaper application for Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [wpaperd](https://github.com/danyspin97/wpaperd) - A wallpaper daemon that shows random wallpapers from a directory and changes them after some time

WIDGETS (BARS, PANELS, ETC.)
----------------------------

- ![TypeScript](https://img.shields.io/badge/typescript-%233178c6.svg?style=plastic&logo=typescript&logoColor=%23faf9f8) [ags](https://github.com/Aylur/ags) - A standalone library for creating GTK-based widgets
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff)&nbsp;![Vala](https://img.shields.io/badge/vala-%237b6ca3.svg?style=plastic&logo=vala&logoColor=fff) [Astal](https://github.com/Aylur/astal) - A framework for creating GTK-based widgets for use with Wayland compositors
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [beanclock](https://codeberg.org/bwbuhse/beanclock) - A simple clock overlay for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [chocobar](https://codeberg.org/notchoc/chocobar) - A simple status bar for wlroots-based Wayland compositors
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [creek](https://github.com/nmeum/creek) - A dwm-inspired fork of levee and minimalist status bar for the River compositor designed to be more malleable by allowing arbitrary text rather than built-in modules
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [dam](https://codeberg.org/sewn/dam) - A small status bar designed for River and wlroots-based Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [deburr](https://github.com/gitRaiku/deburr) - A dwm-like status bar for wlroots-based Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [diowpanel](https://github.com/DiogenesN/diowpanel) - A simple panel for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [diowwindowlist](https://github.com/DiogenesN/diowwindowlist) - A simple GUI application for listing and activating the currently opened toplevels (application windows) in wlroots-based Wayland compositors implementing the `wlr-foreign-toplevel-management-unstable-v1` and `wlr-layer-shell-unstable-v1` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Dvvidget](https://github.com/BL-CZY/dvvidget) - A widget system for Wayland compositors implementing the `wlr-layer-shell-unstable-v1` and `gtk4-layer-shell` protocols
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [dynisland](https://github.com/cr3eperall/dynisland) - An extensible bar for wlroots-based Wayland compositors implementing the `gtk4-layer-shell` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Eww](https://github.com/elkowar/eww) - A standalone widget system that allows for implementing custom widgets in any window manager
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [fabric](https://github.com/Fabric-Development/fabric) - A GTK-based desktop widget framework
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [gBar](https://github.com/scorpion-26/gBar) - A status bar written with GTK
- ![Scheme](https://img.shields.io/badge/scheme-%23000.svg?style=plastic) [greybar](https://codeberg.org/kfu/greybar) - A status bar for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Vala](https://img.shields.io/badge/vala-%237b6ca3.svg?style=plastic&logo=vala&logoColor=fff) [Hybridbar](https://github.com/hcsubser/hybridbar) - A top panel forked from wingpanel for Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [i3status-rust](https://github.com/greshake/i3status-rust) - A resource-friendly and feature-rich replacement for i3status
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [ignis](https://github.com/ignis-sh/ignis) - A widget system based on GTK 4 for Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [Ironbar](https://github.com/JakeStanger/ironbar) - A customizable and feature-rich GTK bar for wlroots-based compositors
- ![Dart](https://img.shields.io/badge/dart-29b6f6?style=plastic&logo=dart&logoColor=01579b)&nbsp;![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [kitshell](https://github.com/bootloopmaster636/kitshell) - A Flutter-based panel for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [levee](https://git.sr.ht/~andreafeletto/levee) - A status bar for the river Wayland compositor, providing support for workspace tags, volume, battery capacity, and screen brightness via built-in modules
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [misiu](https://codeberg.org/saccharin/misiu) - A charming program inspired by xteddy for Wayland compositors implementing the `xdg-shell` protocol
- ![Python](https://img.shields.io/badge/python-4584b6?style=plastic&logo=python&logoColor=ffde57) [nwg-panel](https://github.com/nwg-piotr/nwg-panel) - A GTK 3-based panel for Wayland compositors
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [Root Bar](https://hg.sr.ht/~scoopta/rootbar) - A bar for wlroots-based Wayland compositors such as sway
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [SFWBar](https://github.com/LBCrion/sfwbar) - A flexible taskbar application for Wayland compositors, designed with a stacking layout in mind
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [sysbar](https://github.com/System64fumo/sysbar) - A modular status bar for wlroots-based Wayland compositors, implementing the `gtk4-layer-shell` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [syshud](https://github.com/System64fumo/syshud) - A system status indicator for wlroots-based Wayland compositors, implementing the `gtk4-layer-shell` protocol
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [walrus-bar](https://github.com/elijahimmer/walrus-bar) - A status bar for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Wapanel](https://github.com/Firstbober/wapanel) - A simple panel/status bar/task bar for stacking Wayland-based desktops
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [Waybar](https://github.com/Alexays/Waybar) - A highly customizable bar for Sway and wlroots-based compositors
- ![Rust](https://img.shields.io/badge/rust-%23281c1c.svg?style=plastic&logo=rust&logoColor=fff) [way-edges](https://github.com/way-edges/way-edges) - A lightweight application providing off-screen widgets hidden along the edges of the screen
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wayloadmon](https://git.sr.ht/~leon_plickat/wayloadmon) - A load monitor widget for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wlclock](https://git.sr.ht/~leon_plickat/wlclock) - An analog clock for wlroots-based Wayland compositors, implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wl_shimeji](https://github.com/CluelessCatBurger/wl_shimeji) - A widget overlay for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [wob](https://github.com/francma/wob) - A lightweight overlay volume/backlight/progress/anything bar for wlroots-based Wayland compositors implementing the `wlr-layer-shell-unstable-v1` protocol
- ![Go](https://img.shields.io/badge/go-%2300add8.svg?style=plastic&logo=go&logoColor=fff) [YaGoStatus](https://github.com/burik666/yagostatus) - A replacement for i3status
- ![C](https://img.shields.io/badge/c-%23044f88.svg?style=plastic&logo=c&logoColor=fff) [yambar](https://codeberg.org/dnkl/yambar) - A lightweight and configurable status panel, inspired by polybar
- ![Zig](https://img.shields.io/badge/zig-%23f7a41d.svg?style=plastic&logo=zig&logoColor=fff) [zbar](https://codeberg.org/nwormek/zbar) - A simple status bar for dwl implementing the `wlr-layer-shell-unstable-v1` and `dwl-ipc-unstable-v2` protocols
- ![C++](https://img.shields.io/badge/c++-%235e97d0.svg?style=plastic&logo=c%2B%2B&logoColor=fff) [zenway](https://github.com/2hdddg/zenway) - A sway bar alternative that overlays on top of workspaces
