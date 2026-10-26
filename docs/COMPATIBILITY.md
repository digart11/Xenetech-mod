# Compatibility and Validation

## Tested environment

| Component | Configuration |
| --- | --- |
| Operating system | Windows 11 x64 virtual machine |
| Xenetech executable | Graphic Workstation `6.59.132.3` |
| Original application | Native 32-bit Windows application |
| Modification launcher | Separate 64-bit Windows application |

## Verified tests

| Scenario | Result |
| --- | --- |
| Installation over an existing mod version | Passed |
| Fresh installation | Passed |
| Uninstall and reinstall | Passed |
| Custom running taskbar icon | Passed |
| Shift-click opening another modified instance | Passed |
| Pinning, unpinning, and launching from a taskbar pin | Passed |
| T/Z keyboard shortcuts | Passed |

## Observed behavior

During startup, the original Xenetech icon may briefly appear before the mod's custom icon replaces it.

## Compatibility scope

An installed copy of Xenetech Graphic Workstation is required. These results describe the tested configuration and do not establish support for other application versions, Windows releases, or hardware setups.
