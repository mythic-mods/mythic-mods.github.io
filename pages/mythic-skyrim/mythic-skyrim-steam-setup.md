---
title: Steam Setup
sidebar: mythic-skyrim-sidebar
toc: true
permalink: mythic-skyrim-steam-setup.html
folder: mythic-skyrim
summary: Instructions on preparing a Steam install of Skyrim AE for modlist installation.
---
## Creating a New Steam Library
Skyrim should be installed in a top-level folder that is not in a protected folder.
If you did not install Steam to a UAC protected folder or you already have a Steam Library outside a UAC protected folder, you can skip this step.
Otherwise follow these instructions to create a new Steam Library:
* Open Steam and go into the Settings.
* In the `Downloads` tab, select `Steam Library Folders`.
* Click `Add Library Folder`.
* Point it to a location somewhere outside a UAC protected folder (This should ideally be located on an SSD)
  * Example of good Steam Library location:
    * `G:\Steam Games\`
  * Examples of bad Steam Library locations:
    * `C:\Program Files\`
    * `C:\Program Files x86\`
    * `C:\Users\` (which includes Downloads, Documents, Desktop, etc,)
* Close all windows when you’re done.

## Installing Skyrim
Since all preparations have now been completed, we can install the game through Steam:
* Find Skyrim in your games library and click the Install button.
  * The Anniversary Edition update is fully supported.
* Choose the Steam Library created previously (or your own located outside UAC protected folders) as the location for the install.
* Wait until Skyrim has been fully downloaded and installed before you proceed.

## Steam Settings
In Steam, open the Properties for Skyrim SE and make the following changes:
* In the `Updates` tab, set Automatic Updates to __Only Update This Game When I Launch It__
  * This will prevent Skyrim from updating unless it is manually launched through Steam.
* In the `Language` tab, ensure Language is set to __English__
  * No Wabbajack lists currently support languages other than English.
* In the `General` tab, disable the __Enable the Steam Overlay while in-game__ checkbox.
  * The Steam Overlay can cause issues with some ENB settings and is recommended to disable the feature.

## Initialize Skyrim
Once the game has been installed you will need to launch the game through Steam.
* This is necessary for setting up registry keys and downloading Creation Club content.
* Once all Creation Club content has been downloaded, you can quit from the main menu.
* After this step, you should no longer launch the game through Steam and only launch the game through Mod Organizer 2 to prevent Steam updates.

## Conclusion
After following the steps on this page, you now have a properly prepared Skyrim AE installation that you can install the Mythic Skyrim modlist for.
