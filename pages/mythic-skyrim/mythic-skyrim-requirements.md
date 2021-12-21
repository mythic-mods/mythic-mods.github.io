---
title: Requirements
sidebar: mythic-skyrim-sidebar
toc: true
permalink: mythic-skyrim-requirements.html
folder: mythic-skyrim
summary: The following are required to install and play Mythic Skyrim.
---

## General Requirements

* Latest version of Windows 10 (required by Wabbajack)
* [Skyrim Special Edition] on Steam
* [Skyrim Anniversary Upgrade] on Steam
* [Nexus Mods] account (Premium recommended)


## Disk Space

Mythic Skyrim currently requires ~??GB of free disk space for modlist installation and another ~??GB for the initial downloaded archives.

{% include tip.html content=
"It is recommended to install Mythic Skyrim on an SSD.
The initial installation process will be faster if the downloaded archives are also on an SSD.
They can be moved to a different drive afterwards as they are not necessary for gameplay, only for updating the list.
If you delete them, you will have to redownload them if you want to update so it’s recommended to keep them." %}


## Visual C++ Redistributable

[Microsoft Visual C++] Redistributable is a basic package required by Mod Organizer 2 and typically ships with Windows.
* Download and run the [vc_redist.x64.exe] installer.
* The application will guide you through the installation process.


## Microsoft .NET 5.0

[.NET 5.0 Runtime] framework is required for certain mods. The game will not launch if you do not have it installed.
* Download and run the [Desktop App x64] installer.
* The application will guide you through the installation process.


## Latest GPU Drivers

This is more of a recommendation than a hard requirement, but if you encounter any unexpected performance issues or graphical artifacts it is usually recommended to update your GPU drivers as a first step in troubleshooting. It is highly recommended to update GPU drivers before continuing.
You can find the latest drivers for your GPU on the manufacturers website ([NVIDIA] or [AMD])

{% include tip.html content="For Nvidia, install using the custom option. Select "Peform a Clean Install" option to fully clear old files." %}


[Skyrim Special Edition]: https://store.steampowered.com/app/489830/The_Elder_Scrolls_V_Skyrim_Special_Edition/
[Skyrim Anniversary Upgrade]: https://store.steampowered.com/app/1746860/The_Elder_Scrolls_V_Skyrim_Anniversary_Upgrade/
[Nexus Mods]: https://www.nexusmods.com/
[NVIDIA]: https://www.nvidia.com/Download/index.aspx
[AMD]: https://www.amd.com/en/support
[Microsoft Visual C++]: https://docs.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170
[vc_redist.x64.exe]: https://aka.ms/vs/17/release/vc_redist.x64.exe
[.NET 5.0 Runtime]: https://dotnet.microsoft.com/en-us/download/dotnet/5.0/runtime
[Desktop App x64]: https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-5.0.13-windows-x64-installer
