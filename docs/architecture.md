# ValkOS Architecture

## Base

ValkOS is based on Arch Linux.

## System Stack

Linux Kernel
↓
Arch Linux userspace
↓
systemd
↓
Wayland
↓
Hyprland
↓
ValkOS Desktop Shell
↓
ValkOS Applications

## Existing Components

- Linux kernel
- Arch Linux
- systemd
- pacman
- Wayland
- Hyprland
- PipeWire
- NetworkManager

## ValkOS Components

### Valk Shell

Primary desktop interface.

Responsibilities:

- Panel
- Application launcher
- System tray
- Notifications
- Workspace controls
- Quick settings
- Power controls

### Valk Settings

Graphical system configuration.

### Valk Store

Graphical application discovery and installation.

### Valk Setup

First-boot configuration.

### Valk Update

Graphical system update interface.

### Valk CLI

Command-line interface for ValkOS functionality.

### Valk Installer

Graphical installation environment.

## Build System

The final system should be reproducible from source-controlled
configuration and build scripts.

QEMU will be used for development and automated testing.
