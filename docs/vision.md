# ValkOS

## Vision

ValkOS is an Arch-based Linux distribution designed to make switching
from Windows to Linux as easy and approachable as possible.

The goal is not to hide Linux or turn it into Windows. The goal is to
preserve the flexibility, transparency, and power of Arch Linux while
providing a polished, intuitive, and beginner-friendly experience.

A new user should be able to install ValkOS, connect to the internet,
install applications, configure their hardware, play games, and use
their desktop without needing to understand Linux internals.

Advanced users should still have full access to the underlying Arch
Linux system and its normal tools.

## Design Principles

### 1. Familiar, not a Windows clone

ValkOS should make common Windows workflows intuitive:

- Application launcher
- Taskbar/panel
- File management
- Settings
- Notifications
- Window switching
- Keyboard shortcuts
- System tray
- Software installation
- System updates

The interface should feel familiar without copying Windows visually.

### 2. Sleek and responsive

The desktop should prioritize:

- Smooth animations
- Fluid transitions
- Minimal visual clutter
- Consistent design
- Subtle transparency and effects
- Clear visual hierarchy
- Fast interaction

The interface should feel modern without becoming resource-heavy.

### 3. Arch underneath

ValkOS should remain recognizably Arch Linux underneath the ValkOS
experience.

Prefer existing, proven components rather than unnecessarily
reimplementing them.

Core components:

- Linux kernel
- Arch Linux userspace
- systemd
- pacman
- Wayland
- Hyprland
- PipeWire
- NetworkManager

### 4. GUI first, terminal always available

Common operations should have graphical interfaces.

The terminal should never be hidden or restricted.

Users who want to use pacman, systemctl, journalctl, configuration
files, and other Linux tools should be able to do so normally.

### 5. Reduce the Arch tax

ValkOS should automate or simplify common tasks that traditionally
require manual Arch configuration.

Examples:

- Installation
- Hardware configuration
- GPU setup
- Network configuration
- Audio configuration
- Bluetooth
- System updates
- Application installation
- Gaming setup
- Development environment setup
- Recovery and troubleshooting

### 6. Gaming friendly

ValkOS should provide a strong gaming experience without requiring
users to manually configure a large collection of tools.

Potential components include:

- Steam
- Proton
- Vulkan
- Gamescope
- GameMode
- MangoHud
- Controller support
- Wine and compatibility tools

Gaming components should remain optional where appropriate.

### 7. Development friendly

ValkOS should also function as a serious development workstation.

Potential development profiles include:

- Git
- GCC
- Clang
- CMake
- Ninja
- Python
- Node.js
- Rust
- Blender
- Godot
- Vulkan development tools

Users should be able to install these through the graphical software
system or the terminal.

## ValkOS Components

Components we intend to build ourselves:

- Valk Shell
- Valk Settings
- Valk Store
- Valk Installer
- Valk Setup
- Valk Update
- Valk CLI
- Valk hardware/configuration utilities
- ValkOS package repository
- ValkOS ISO/build system

## Technical Philosophy

ValkOS should avoid replacing mature Linux infrastructure without a
strong reason.

If an existing component works well, ValkOS should integrate with it.

Examples:

- Linux instead of a custom kernel
- Hyprland instead of a custom compositor
- systemd instead of a custom init system
- pacman instead of a custom package manager
- Wayland instead of a custom display protocol

ValkOS should focus its engineering effort on integration, usability,
automation, and the desktop experience.

## Reproducibility

The complete operating system should eventually be reproducible from
a version-controlled repository.

The goal is to be able to:

1. Build ValkOS packages.
2. Build the ValkOS system.
3. Generate an installation ISO.
4. Boot the ISO in QEMU.
5. Install ValkOS.
6. Run automated tests.
7. Produce a release.

## Initial Milestone

The first milestone is not a finished distribution.

The initial goal is to create a controlled Arch Linux development
environment in QEMU and progressively build ValkOS on top of it.

The first major user-facing milestone will be:

> A clean Arch-based system running Hyprland with the first ValkOS
> desktop components.

## Long-Term Goal

ValkOS should demonstrate that an Arch-based Linux system can retain
the flexibility and power of Arch while providing an experience that
a Windows user can understand immediately.
