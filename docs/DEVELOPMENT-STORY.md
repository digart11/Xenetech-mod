# Development story

## Why this project exists

Many long-lived desktop applications remain valuable because of their mature workflows and specialized capabilities. At the same time, their interfaces can feel out of step with modern Windows conventions. Xenetech digART Edition began as an exploration of how to improve that experience without replacing the original software.

## From interface changes to a complete desktop integration

The effort developed beyond visual styling into practical quality-of-life improvements: more convenient controls, keyboard changes, workflow enhancements, printing-related refinements, and its own launch/install experience.

A particularly instructive Windows issue appeared near the end: the custom desktop shortcut opened the modified application, but the Windows taskbar still showed the original application identity. Shift-click therefore opened a native, unmodified instance instead of another digART instance.

The eventual solution involved treating the taskbar as an application-identity problem rather than simply an icon problem. The final candidate was tested with the custom running icon, taskbar grouping, Shift-click multi-instance relaunch, and pinning.

## Validation and release milestone

The finished v1.0 milestone was validated in a clean Windows 11 VM, both as an upgrade over an earlier digART installation and as a fresh installation after uninstalling. The verified installer was retained unchanged after acceptance testing, while earlier builds and test evidence were archived privately.

## A note on scope

This account describes the public-facing project history, not a complete reverse-engineering diary. Sensitive implementation and third-party licensing material remain private.
