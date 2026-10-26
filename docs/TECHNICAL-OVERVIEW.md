# Technical Overview

## Design

Xenetech digART Edition Mod extends the existing Xenetech Graphic Workstation application without permanently modifying its original executable. A separate launcher, runtime enhancements, and installer provide the modified experience while keeping the original application installation intact.

## Components

| Component | Function |
| --- | --- |
| Mod launcher | Starts the installed Xenetech application with the enhancement environment |
| Runtime enhancement layer | Applies interface and workflow refinements during execution |
| Interface and window branding | Updates selected native UI elements and the application's visible identity |
| Windows desktop integration | Coordinates shortcuts, running-window identity, taskbar grouping and relaunch |
| Custom installer | Installs and uninstalls the mod separately from Xenetech |

## Native application integration

Xenetech Graphic Workstation is a native 32-bit Windows application. The mod uses a separate 64-bit launcher to coordinate startup and the runtime enhancement layer. This architecture preserves the existing executable while adding functionality around it.

## Taskbar identity and multiple instances

The application's visible windows are owned by the original Xenetech process. At first, Windows displayed the original icon and used the original executable when opening another instance from the taskbar.

The mod coordinates the running window's Windows Shell identity with its own launcher and installed shortcuts. This allows modified windows to group correctly and supports pinned launching and Shift-click multi-instance launching.

## Workflow compatibility

The runtime enhancements coexist with the application's native controls, keyboard handling, printing workflow, and normal window shutdown. Compatibility was checked through targeted tests and Windows 11 installation scenarios.

## Installation and removal

The custom installer installs the modification as a separate Windows application. Both upgrade and fresh-install scenarios were tested, including removal and reinstallation, without replacing the original Xenetech executable.
