<div align="center">

# Xenetech digART Edition Mod

**A redesigned interface and enhanced workflows for Xenetech Graphic Workstation**

Dark interface · Quick-access tools · Printing enhancements · Windows integration

**Windows 11 x64** · **Xenetech 6.59.132.3** · **Version 1.0**

**Created by digART**

</div>

## Overview

**Xenetech digART Edition Mod** is an independent modification of the Xenetech Graphic Workstation experience. It refreshes the interface with a consistent dark appearance and introduces practical improvements to everyday editing, printing, and application controls.

The mod works alongside an existing Xenetech installation. Its dedicated launcher applies the enhancements while preserving the original application executable, and its separate installer allows the mod to be installed or removed independently.

## Main interface

![Xenetech digART Edition Mod — redesigned main workspace](screenshots/main-interface.png)

The redesigned workspace brings darker styling and refined interface elements to the familiar Xenetech environment, retaining the underlying tools and workflow.

## Features and improvements

### Printing window and quick settings

![Xenetech digART Edition Mod — printing window and quick settings](screenshots/printer-window.png)

Improved access to selected print controls makes it easier to adjust settings while preparing output, without repeatedly navigating through the original interface.

### Toolbar and quick tools

![Xenetech digART Edition Mod — toolbar and quick tools](screenshots/toolbar-tools.png)

Quick-access toolbar actions simplify routine operations. Additional refinements cover selected native Frame and Border workflows.

### Keyboard shortcuts

![Xenetech digART Edition Mod — keyboard shortcuts](screenshots/shortcuts.png)

Updated shortcut handling supports efficient navigation and editing while preserving ordinary text input, including compatible T/Z shortcut behavior.

### Windows desktop integration

The mod has its own application icon and dedicated desktop and Start Menu shortcuts. Its taskbar identity supports pinning, proper grouping of modified windows, and **Shift-click to open another modified instance**.

### Custom installer

![Xenetech digART Edition Mod — installer](screenshots/installer.png)

The custom installer provides a branded setup experience, supports installation over an existing mod version, and includes independent uninstall support.

Read the [detailed feature overview](docs/FEATURES.md).

## Engineering overview

The project combines a dedicated launcher, a runtime customization layer, native Windows integration, and modular interface and workflow enhancements. The original Xenetech executable remains unchanged.

A notable engineering challenge was making the running Xenetech window use the mod's taskbar identity. Correcting this enabled the custom taskbar icon, pinned launching, and Shift-click multi-instance behavior without redirecting users into an unmodified Xenetech session.

See the [Technical Overview](docs/TECHNICAL-OVERVIEW.md) and [Development Story](docs/DEVELOPMENT-STORY.md).

## Compatibility

| Component | Verified configuration |
| --- | --- |
| Operating system | Windows 11 x64 |
| Original application | Xenetech Graphic Workstation executable `6.59.132.3` |
| Architecture | Native 32-bit application with a separate 64-bit mod launcher |
| Installer | Upgrade, fresh installation, uninstall and reinstall |
| Taskbar | Custom icon, pinning and Shift-click multi-instance launching |
| Keyboard | T/Z shortcuts and normal typing |

An existing Xenetech installation is required. Testing on additional application builds and Windows versions has not been established. See [Compatibility and Validation](docs/COMPATIBILITY.md).

## Documentation

- [Features and Improvements](docs/FEATURES.md)
- [Technical Overview](docs/TECHNICAL-OVERVIEW.md)
- [Development Story](docs/DEVELOPMENT-STORY.md)
- [Compatibility and Validation](docs/COMPATIBILITY.md)
- [Project Status](docs/STATUS.md)

## Availability

This repository presents the Xenetech digART Edition Mod project and its features. The installer and production source code are not distributed through this repository.

## Disclaimer

Xenetech digART Edition Mod is an independent, unofficial project created by digART. It is not affiliated with, sponsored by, or endorsed by Xenetech. All third-party product names and trademarks remain the property of their respective owners. See the [full disclaimer](DISCLAIMER.md).
