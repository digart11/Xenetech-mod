# Compatibility and validation

## Tested configuration

- Windows 11 x64 virtual machine.
- Xenetech Graphic Workstation native executable version `6.59.132.3`.
- digART independent x64 launcher controlling an installed x86 application.

No claim is made that all Xenetech builds, other Windows versions, or different system configurations are supported.

## Observed acceptance tests

| Scenario | Result |
| --- | --- |
| Upgrade installation over existing digART installation | Passed |
| Fresh install following digART uninstall | Passed |
| Uninstall and reinstall | Passed |
| Custom running taskbar icon | Passed |
| Shift-click opening another modified instance | Passed |
| Taskbar pin/unpin and launch from pinned entry | Passed |
| T/Z keyboard shortcuts | Passed |

## Known observation

The original red Xenetech icon may appear briefly during startup and is replaced by the digART icon once runtime branding has initialized.

## Notes

These results reflect the observed test environment at the time of the v1.0 project milestone. They do not constitute independent certification or a guarantee on other machines.
