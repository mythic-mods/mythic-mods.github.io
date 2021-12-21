---
title: Installation
sidebar: mythic-skyrim-sidebar
toc: true
permalink: mythic-skyrim-installation.html
folder: mythic-skyrim
summary: Instructions on installing Wabbajack and the Mythic Skyrim modlist.
---

{% include important.html content="Ensure you have followed the steps outlined in [Steam Setup] before proceeding with installation." %}


## Wabbajack Installation

Wabbajack should be installed to a top-level folder that is not <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.uac}}">UAC</a> protected in the same way you setup your Steam Library in previous steps.
* A top-level folder such as `G:\Wabbajack\` is once again recommended as the installation directory.
* Create a new top-level folder in a location that is not UAC protected and name it `Wabbajack`

Download the [Wabbajack] application directly from the website: 
* Click the `Download` button on the home page of the Wabbajack site.
* Move the downloaded `Wabbajack.exe` into the `Wabbajack` folder you previously created.
* Double-click `Wabbajack.exe` to launch the application.
* When launched, Wabbajack will be automatically updated to the latest version and downloaded into the same directory.


## Mythic Skyrim Installation

You can now install Mythic Skyrim through Wabbajack:
* Click the `Browse Modlists` button in the Wabbajack tool.
* Find Mythic Skyrim in the gallery of mod lists and click the arrow button to download the installation file.
* In the installation window, you will need to define two folders:
  * Installation Location is where Mythic Skyrim will be installed to. Choose a high-level folder such as `G:\Mythic Skyrim\` that is outside UAC protected folders (Program Files, Documents, etc).
  * Download Location is where the downloaded mod archives will be stored. By default, they will be placed within your main Mythic Skyrim folder, but you can change the file path if you want to keep the files elsewhere.
* Once both folder locations have been set, click the button on the right to begin the installation process. 


### Nexus Mods Downloads

If you have a Nexus Premium account, Wabbajack will automatically download and install all mods from the Nexus Mods website in the modlist for you.

If you only have a free Nexus account, Wabbajack will open the Nexus mod pages for you and guide you through the process of downloading all files.
Afterwards, it will proceed with the installation as usual.

{% include tip.html content="A Nexus Premium account is highly recommended." %}


### Installation Process

As Wabbajack downloads the modlist, previews will be displayed of the mods being installed.
Unless the installation is aborted completely, you don’t have to worry about any warnings.
You will be prompted when the installation process is complete.

### Troubleshooting Installation
In the case of a failed installation: restart Wabbajack. You will not lose progress as the tool will pick up where it left of.
You can find all Wabbajack logs in your Wabbajack installation folder under `\Wabbajack\logs\`.


[Wabbajack]: https://www.wabbajack.org/#/
[Steam Setup]: mythic-skyrim-steam-setup.html
