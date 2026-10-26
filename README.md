<div align="center">

# Xenetech digART Edition

**An independent modernization project for Xenetech Graphic Workstation**

*Updated interface · Faster everyday workflows · Native Windows integration · Independent installation*

**Windows 11** · **Xenetech 6.59.132.3** · **Project milestone: v1.0**

</div>

> [!NOTE]
> **Project showcase.** This repository documents an independent, privately developed modification. It does not contain the modification's production source code, third-party software, or an installer download. Xenetech Graphic Workstation is a separate product and is required for the modification to operate.

## Overview

Xenetech digART Edition is a personal engineering project exploring how an established Windows graphics workstation can be modernized **without permanently modifying its original executable**.

The project introduces interface refinements, additional workflow controls, keyboard improvements, printing-related enhancements, a dedicated launcher, and a custom installation experience. It also integrates with Windows taskbar identity and relaunch behavior so multiple modified instances can be opened using normal Windows interactions.

The goal is not to replace Xenetech. It is to make selected everyday interactions with the existing application more consistent and convenient, while keeping the underlying installation separate.

## Interface preview

<!-- Replace this line with an image when screenshots/main-interface.png is provided. -->
**Main interface screenshot — coming soon**

The screenshots below will be added after personal and customer information is removed.

## What changed

| Area | Improvements |
| --- | --- |
| **Main interface** | A redesigned dark presentation and refinements to the working environment |
| **Printing workflow** | Additional controls and quicker access to selected printing settings |
| **Toolbar & quick tools** | Faster access to useful workflow actions, including native tool enhancements |
| **Keyboard** | Improved shortcut handling, including T/Z behavior and normal typing compatibility |
| **Windows integration** | Dedicated icon and shortcuts, taskbar grouping, pinned launching, and Shift-click multi-instance relaunch |
| **Installation** | A separate branded launcher and installer with uninstall support |

For more details, see [Features](docs/FEATURES.md).

## Gallery

Screenshots will document the actual tested interface:

1. **Main workspace** — the primary UI and dark visual design.
2. **Printer window** — added controls and quick settings.
3. **Toolbar** — quick tools and enhanced workflow controls.
4. **Shortcuts** — keyboard shortcut reference and behavior.
5. **Installer** — the custom setup experience.

Images will be stored in [`screenshots/`](screenshots/README.md). This repository intentionally avoids mockups presented as actual software captures.

## How it works — at a high level

```text
User launches digART Edition
          |
          v
    digART launcher
          |
          v
Installed Xenetech application
          |
          v
Runtime UI and workflow enhancements
          |
          v
Modernized Xenetech experience
```

The project uses a separate launcher and runtime customization layer, rather than redistributing a modified Xenetech executable. The actual implementation, native hooks, internal offsets, and private research are not published here.

Read the [Technical Overview](docs/TECHNICAL-OVERVIEW.md) for a non-sensitive architecture explanation.

## Compatibility and project status

- **Tested environment:** Windows 11 x64.
- **Tested application:** Xenetech Graphic Workstation executable version **6.59.132.3**.
- **Application architecture:** native 32-bit target, with a separate 64-bit launcher.
- **Verification:** upgrade installation, fresh installation, uninstall/reinstall, desktop and pinned launching, custom taskbar icon, Shift-click opening another modified instance, and T/Z shortcuts were tested successfully in a Windows 11 VM.
- **Known minor cosmetic behavior:** the original red application icon can appear briefly during startup before the custom icon takes over.

**This is a documented project milestone, not a claim of universal compatibility or a public support commitment.**

## Project notes

- [Features and screenshots](docs/FEATURES.md)
- [Technical overview](docs/TECHNICAL-OVERVIEW.md)
- [Development story](docs/DEVELOPMENT-STORY.md)
- [Compatibility and testing](docs/COMPATIBILITY.md)
- [Project status and distribution](docs/STATUS.md)
- [Disclaimer and rights](DISCLAIMER.md)

## Availability

This is currently a **documentation/showcase repository**. The production implementation, licensing-related research, and installer are not included. Any decision to distribute binaries or publish selected source examples will be made separately after a rights and security review.

## Disclaimer

Unofficial independent project. Not affiliated with, sponsored by, or endorsed by Xenetech. All third-party product names and trademarks belong to their respective owners. See [Disclaimer](DISCLAIMER.md).
