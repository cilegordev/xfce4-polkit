Xfce4-Polkit
===========

A simple policykit authentication agent for xfce4

<a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-GPL%20v2-orange"></a>
<a href="https://github.com/cilegordev/xfce4-polkit/releases"><img src="https://img.shields.io/github/v/tag/cilegordev/xfce4-polkit.svg"></a>
<a href="https://repology.org/metapackage/xfce-polkit"><img src="https://repology.org/badge/tiny-repos/xfce-polkit.svg" alt="Packaging status"></a>

# Required Packages

Xfce4-Polkit depends on the following packages:

- glib
- libxfce4ui
- polkit

# Installation

Run the following commands at the root of the repository:
```
mkdir build
cd build
meson .. --prefix=/usr
ninja
```
to compile, then run
```
ninja install
```
as root to install.

# Usage
Make sure there's no other policykit authentication agent running (if there is, `kill` them.)
If you wish to use this by default, make sure `xfce4-polkit` is the only authentication agent that is run at boot.
