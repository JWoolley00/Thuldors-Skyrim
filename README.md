![](https://github.com/JWoolley00/Thuldors-Skyrim/blob/main/thuldor's%20skyrim.jpg)

<p align="center">
  [ <a href="https://www.nexusmods.com/users/134860433?tab=user+files">Nexus</a> |
    <a href="https://www.nexusmods.com/users/134860433?tab=user+files">Installation</a> |
    <a href="https://www.nexusmods.com/users/134860433?tab=user+files">Features</a> | 
    <a href="https://www.nexusmods.com/users/134860433?tab=user+files">Changelog</a> | 
    <a href="https://www.nexusmods.com/users/134860433?tab=user+files">Modlist</a> ]
</p>

---

# Attention

**Thuldor's Skyrim requires the full AE upgrade, which means you must purchase the AE edition of the game for the list to function.**

**You must update Skyrim to the latest version (1.6.1170) on Steam to install this list.**

# Contents
- [Attention](#attention)
- [Contents](#contents)
  - [Introduction](#introduction)
    - [System Requirements](#system-requirements)
  - [Installation](#installation)
    - [Pre-Installation](#pre-installation)
      - [Installing Microsoft Visual C++ Redistribution Package](#installing-microsoft-visual-c-redistribution-package)
      - [Pagefile and crash prevention](#pagefile-and-crash-prevention)
      - [Setting Shader Cache Size](#setting-shader-cache-size)
      - [Steam Setup](#steam-setup)
      - [Game Language](#game-language)
      - [Installing Creation Club Content](#installing-creation-club-content)
    - [Wabbajack Installation](#wabbajack-installation)
      - [Installing Wabbajack](#installing-wabbajack)
      - [Downloading and Installing Thuldor's Skyrim](#downloading-and-installing-thuldors-skyrim)
    - [Problems with installation](#problems-with-installation)
  - [Post-Installation](#post-installation)
    - [Game Folder](#game-folder)
    - [Antivirus Exceptions](#antivirus-exceptions)
    - [Controller and Gamepad Setup](#controller-and-gamepad-setup)
  - [Updating the modlist](#updating-the-modlist)
  - [Removing the Modlist](#removing-the-modlist)
  - [Issues](#issues)
  - [Credits and Thanks](#credits-and-thanks)

## Introduction

Thuldor's Skyrim is just that - a personalized load order I've developed for about one year, brought to you in an easy-to-install package. You'll find enhanced visuals, new quests, grander locations, and more rewarding gameplay, all integrated into a cohesive experience that remains faithful to the original game.

The full modlist can be viewed [here](https://www.nexusmods.com/users/134860433?tab=user+files).

You can find a summary of all relevant changes on the [Gameplay Guide](https://www.nexusmods.com/users/134860433?tab=user+files).

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

### System Requirements

>  Please note these specs are the best idea of a baseline that I can provide at the current moment, based on feedback I have gotten from testers and my own experiences. In the future this will be updated depending on feedback received.


| Spec Category | My Specs (1440p) | Recommended (1080p) |
|     :---:    |     :---:     |     :---:     
| **CPU**   | R5 5600 |  R7 3700x / i5 10600k |
| **Video Card**    | RX 6700XT | 3060 Ti / 2070 / 6700 XT |
| **Ram**    | 32gb (4x8) | 16gb (2x8) |
| **Storage**    | 970 EVO NVMe | SATA SSD |

Please note that the below numbers are current estimates and the actual may be larger or smaller depending on version.

Downloads: ~95 GB  
Install: ~250 GB    

 > Wabbajack requires around 30 GB of space on your main OS drive for temporary and working files during the installation, this space is not counted towards the total install space of the list for sake of this guide, however Wabbajack roughly accounts for it in the UI.

## Installation

Installing Thuldor's Skyrim is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

### Pre-Installation

<Details>
<summary>Pre-Installation Instructions</summary>

These steps are only required for installing the Modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

#### Installing Microsoft Visual C++ Redistribution Package

 1. Install [Visual C++ x64](https://aka.ms/vs/16/release/vc_redist.x64.exe) & [.Net Runtime v6 desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
 2. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 3. Right click on Skyrim SE and click on properties, untick the "Enable Steam Overlay while in-game."
 4. You also need to start the games to the main menu in order to download all the creations. **DO NOT SKIP THIS STEP, IF YOU DO SO WABBAJACK WILL FAIL**

#### Pagefile and crash prevention

Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. Due to its size and number of files required to be handled for the list, this step is **NOT** optional, I do not care how much RAM or VRAM you have, please do this step.

 To set up your pagefile:
 1. Press **Win Key + R**
 2. Type *sysdm.cpl ,3* and hit **ENTER**
 3. Navigate to *Performance* and click the box "Settings..."
 4. Click the *Advanced* tab at the top
 5. Under *Virtual Memory* click the box "Change..."
 6. Uncheck *Automatically manage* if it is checked
 7. Select your disk drive, ideally your fastest solid state drive
 8. Click the **Custom size:** button
 9. In the box next to **Initial Size (MB)** type `40960`
 10. In the box next to **Maximum Size (MB)** type `40960`
 11. Click the *Set* button
 12. Click *OK*
 13. Click *Apply*
 14. Click *OK*
 15. Restart your computer in order for your new pagefile to take effect.

#### Setting Shader Cache Size
 Additionally, if you have an NVIDIA GeForce Graphics Card, please do the following: 

 1. Right-click on your desktop and select **NVIDIA Control Panel**
 2. Navigate and click on **Manage 3D settings**. It is the 2nd one to the top.
 3. Scroll down in Global Settings until you see **Shader Cache Size**
 4. Double Click **Driver Default** to the right of Shader Cache Size and select **10 GB**
 5. Click **Apply** in the bottom right hand corner. 
 6. You may exit out of the application.
![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

#### Steam Setup

 If you have your Steam Library in Program Files, read [this](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) and move it elsewhere. Locations such as Desktop, Documents, Downloads, OneDrive, etc. will cause issues with installing and playing the list.

#### Game Language

The English Steam version of Skyrim is the only supported version. I understand that this may be frustrating for non-English speaking users or users with the GOG/Bethesda.net versions, but due to the core file differences between the different versions, I am only able to support one game version.

 1. Right click on your Skyrim in Steam
 2. Click *Properties*
 3. Click *Language*
 4. Set the Language to English.

#### Installing Creation Club Content

 If you have never installed the Creation Club Content before, please do the following:
 1. Purchase the *Skyrim Anniversary Edition* Upgrade from Steam. If you do not do this, you can not install or play the list. 
   > **There is no work around for this and pirating this content will not work. If you pirate the content and come asking for assistance, you will be banned.**
 2. Once you have the Anniversary Edition bought, do the following steps below.
 3. In your Steam Library, right-click on the menu entry for Skyrim, select `Properties` and then select `Local Files`. Click `Verify Integrity of Game Files` and wait.
 4. Once this is completed, launch the game once from Steam. You may receive a prompt that your settings were detected or not detected, this does not matter, nor do any options you select here. Simply open the launcher and launch the game.
 5. Once the intro logo finishes displaying and the Skyrim logo appears, you should receive a prompt to "Download All Content?" Accept this option.
 6. If you did not receive a prompt to download, select the Creation Club option from the menu, and you should find a "Download All" prompt in there somewhere. If this message does not appear, you have not purchased the $20 Upgrade. Begin again from step 1.
 7. Wait for the download process to complete. Do **NOT** ALT-TAB during this process as it will cause the process to fail and you will have to start over again.
 8. Proceed with the rest of the installation.

</Details>

### Wabbajack Installation

<Details>
<summary>Wabbajack Installation Instructions</summary>

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases) on this github and place it in a folder such as `C:\Wabbajack`. **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**. I recommend placing it on an SSD as it will work quicker on there.

The list requires Wabbajack version **3.5.0.1 or later**, installing on older versions of Wabbajack will prevent the installation from being completed.

#### Downloading and Installing Thuldor's Skyrim

Downloading and installing Thuldor's Skyrim can take a while depending on your internet connection and computer. To install Thuldor's Skyrim, complete the following steps.

1. Open Wabbajack and click `Browse Modlists`
2. Press the download button on Thuldor's Skyrim and wait for it to download.
3. Set the installation folder to be somewhere like C:\Games\Thuldor's Skyrim. **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, etc.), or in your Skyrim's Steam folder**
> The download location does not need to be on a SSD, but it makes installing faster.
4. Press the play button to begin.
5. Turn on your favorite show or a nice long video essay Wabbajack does its thing. Alternatively read through this readme again.
6. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow what is below and review the instructions above for any missed steps.

</Details>

### Problems with installation

<Details>
<summary>Troubleshooting Installation Instructions</summary>

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

- Could not download **X**:
	- Big files can fail to download due to connection issues. You can either run wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads.

- **X** is not a whitelisted download:

	 - This may happen when I update the modlist. Please check if there is a new update or wait until you see a release ping.

- Wabbajack could not find my game folder:

	- Either buy the game or go back to the [Pre-Installation](#pre-installation) step.

- Antivirus reports a virus:
	- Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. You can fix this by [adding an exclusion for Mod Organizer in windows defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

- Unable to download `Data_ccXXXXX - *.bsa` or `*.esp`:
	- This error means that there is an issue where Wabbajack is unable to hash your Creation Club Content. If you have followed the steps outlined under [Pre-Installation](#installing-creation-club-content), are not on a pirated copy of the game, and have verified your steam files, then it is very likely that Wabbajack or Bethesda has messed up the hashing for these files. If this is the case, please wait for it to be resolved before continuing to download the list.

- Unable to download `Skyrim_Default.ini`:
 - This error means you failed to follow the readme. Go back to the [game language](#game-language) section and set your game language to English.

</Details>

## Post-Installation

<Details>
<summary>Post-Installation Information</summary>

### Game Folder

Thuldor's Skyrim uses a Wabbajack feature called Stock Game to keep your Skyrim installation clean. All the files that you need to run the list are in a folder called `Stock Game`. You don’t need to copy anything at all.

### Antivirus Exceptions

Generally speaking, using Windows Defender is advised as it is a solid antivirus software that will have minimal interference with the game. Antivirus programs can be notorious for false flagging MO2's VFS as problematic, causing crashes or other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will very likely need to fully remove them from your PC in order to actually launch the game through MO2.

If you use Windows Defender, it is advised that you set up an Exception for the modlist. To do this follow these steps.
 1. Press the Windows Key.
 2. Type "Windows Defender" in the search bar and select "Windows Security".
 3. Click on "Virus & threat protection" in the left pane.
 4. Click the "Manage settings" option under "Virus & threat protection settings".
 5. Scroll down to "Exclusions" and click "Add or remove exclusions".
 6. Windows Defender will prompt you with a run as administrator screen, just hit yes.
 7. Click the "Add an exclusion" button at the top and choose "Folder".
 8. Navigate to your Install folder for the list and click "Select Folder".
 9. **(OPTIONAL)** You can repeat these steps for the other executables:
    - ModOrganizer.exe (`[Path to Modlist]\ModOrganizer.exe`)
    - Nemesis Unlimited Behavior Engine.exe (`[Path to Modlist]\mods\Project New Reign - Nemesis Unlimited Behavior Engine\Nemesis_Engine\Nemesis Unlimited Behavior Engine.exe`)
    - Synthesis.exe (`[Path to Modlist]\tools\Synthesis\Synthesis.exe`)

### Controller and Gamepad Setup

The list currently offers minimal gamepad support, this section will be updated in the future when gamepad support is improved.

## Updating the modlist

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.
 - `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
 - `MINOR`: Any release with a number change here will be considered a minor update, these updates will usually not be save safe, unless otherwise specified.
 - `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
 - In some rare cases you may see a fourth slot be used, which I will refer to as `HOTFIX`. These list "updates" will be used if the list needs to be recompiled for any reason. There will be no changes in these "updates" as they are purely for maintenance.
Before updating, please check the [changelog](https://www.nexusmods.com/skyrimspecialedition/images/227751) and back up your saves. You may need to start a new game after certain updates.
Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite existing modlist` button. **Note**: Any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with **[NoDelete]**.

**ALWAYS** back up saves, control preferences, and any RaceMenu presets before an update. 

*Please make sure you back up your saves if you plan on continuing a playthrough across a **save safe** update.*

</Details>

## Removing the Modlist
Simply delete the folder. Congratulations, you have uninstalled Thuldor's Skyrim.

## Issues

If you encounter any bugs or issues while playing the list, leave a bug report on the [Nexus Page](https://www.nexusmods.com/skyrimspecialedition/images/227751)

By necessity, updates will be infrequent.

## Credits and Thanks

- _YOU_ for reading this.
- Bethesda Game Studios for Skyrim and the Creation Kit.
- Melcin and RustyNails, for your many, many hours of playtesting.
- [Aljixo](https://www.nexusmods.com/skyrimspecialedition/users/68019769) for lending this GitHub documentation format. 
- [ElminsterAU](https://www.patreon.com/ElminsterAU) and the xEdit team for SSEEdit.
- [Noggog](https://www.nexusmods.com/skyrim/users/862590) for Mutagen and Synthesis.
- [Halgari](https://www.nexusmods.com/skyrimspecialedition/users/17252164) and the WJ Team for the amazing platform that is Wabbajack.
- [Sheson](https://ko-fi.com/sheson) for DynDOLOD.
- The Simon Makes Mods Discord for providing a community off of which to bounce my ideas.
