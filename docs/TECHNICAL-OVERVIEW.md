# Technical overview

## Engineering objective

Extend the user experience of an older native Windows application while minimizing changes to its on-disk installation. The approach separates the original application from the independently maintained launcher, enhancement modules, and installer.

## High-level components

| Component | Responsibility |
| --- | --- |
| Launcher | Starts the installed application through the digART workflow |
| Runtime customization | Adds selected interface and workflow behavior within the running application |
| UI/branding layer | Applies visual changes and custom window branding |
| Windows integration | Aligns installed shortcuts and taskbar identity with the digART launcher |
| Installer | Deploys the modification separately and supports removal |
| Verification | Checks packaged artifacts and tests behavior in isolated Windows environments |

## Interesting challenges

### Crossing process architectures

The original application is a 32-bit native Windows program, while the independent launcher is 64-bit. Making the two cooperate requires careful attention to Windows process and window behavior.

### Real application windows versus the launcher

The application window is owned by the native Xenetech process. Windows initially treated it as that original executable for taskbar icon and relaunch operations. The project addressed that mismatch by coordinating the launcher, shortcuts, and the running application's Windows Shell identity.

### Multi-instance behavior

Launching the modified application twice from its desktop shortcut worked, but taskbar Shift-click originally followed the native executable path. The final project milestone tested corrected taskbar relaunch behavior and multiple modified instances on Windows 11.

### Maintaining existing behavior

Enhancements to keyboard handling, printing, native tools, and application redraw required targeted regression checks. Isolation and repeatability were important: a visible UI improvement should not break unrelated normal application interactions.

### Installer repeatability

The project was verified in both upgrade and fresh-install scenarios, including removal and independent launching from Windows shortcuts and taskbar pins.

## What is intentionally excluded

This document does **not** publish:

- Runtime injection scripts or production controller/launcher source.
- Reverse-engineered addresses, binary offsets, or hook signatures.
- Proprietary application files or decompiled code.
- License/registration research, backups, keys, or bypass procedures.
- Private build tools, internal dependency bundles, or sensitive logs.

This repository is a technical presentation of the project, **not** a set of instructions for reproducing its internals.
