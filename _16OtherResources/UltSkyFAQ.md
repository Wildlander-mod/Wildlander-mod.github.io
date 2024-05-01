---
layout: default
title: Ultimate Skyrim FAQ
description: Ultimate Skyrim - Frequently Asked Questions
parent: Ultimate Skyrim
---
	
## Table of contents
{: .no_toc }
<details markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>


## Does this mod pack support SSE?

### Does this mod pack support SSE/AE?
Ultimate Skyrim is only for Legal copies of Skyrim Classic Edition w/ All DLC’s, otherwise known as Skyrim Legendary Edition.

### Where can I buy legendary Edition?
You can buy Legendary Edition from one of the places linked in Wabbajack's Reddit post:

[Wabbajack:How to get Skyrim LE in 2021](https://www.reddit.com/r/Wabbajack/comments/kx6ppr/how_to_get_skyrim_legendary_edition_in_2021/)

---
## How Do I Update to the current Version.
Please note the 4.3 is not save game compatible. Updating will require a fresh game with new MCM setup.

You would delete the contents of your _Ultsky install folder_\content With the exception to downloads.
	
Then you follow the install guide from step 2.3 [here](https://wiki.wildlandermod.com/16OtherResources/UltimateSkyrim/)
	
---
	
## How do I Uninstall?
	
Were sorry to see you leave!
	
Removing Ultsky is a simple matter of removing the files from your steam Skyrim folder that you copied from game folder files(below). Then deleting the Ultimate Skyrim installation folder.
	
![image](https://user-images.githubusercontent.com/26418143/124308354-1674dc00-db61-11eb-92d5-11ff65d4e601.png)
	
---
## **Wabbajack Issues**

### Wabbajack Fails to install with GameFileSourceDownloader Error
If you have Wabbajack Fail with the messages containing GameFileSourceDownloader

There are Four Known causes

1) You have Skyrim installed in program files

	Solution: Close and Run Wabbajack installer as a administrator.
	
2) You have previously "cleaned" your DLC.

	Solution: Have steam verify the game files. 
	
3) You have moved your Skyrim Install from where you originally installed it.

	Solution: Move it back, and use steam to move it to the new location.
	
4) You don't have the DLC installed.

	Solution: Install it, if you don't own it you can find a link to purchase it here [Wabbajack:How to get Skyrim LE in 2021](https://www.reddit.com/r/Wabbajack/comments/kx6ppr/how_to_get_skyrim_legendary_edition_in_2021/) .
	
After doing the solution 2,3  or 4, you will need to restart Wabbajack.

---
### Wabbajack Fails to download mods or hangs for a long time.

Sometimes Wabbajack gets stuck downloading.

1. Close and restart Wabbajack - Start the Ultimate Skyrim install process again, entering same criteria as originally. Wabbajack will the CRC check your existing files and will normally resume where it failed & complete the install without any further intervention.
2. If that does not resolve the issue, try using a VPN service such as Cloudflare WARP or ProtonVPN. (Ultimate Skyrim is not affiliated with and does not endorse any specific VPN service. We does not provide user support for VPN services. Use at your own discretion.)

---
## **Current Version Issues**

### Can't Launch Ultimate Skyrim Bat file
Symptom: a screen flashes up for a half a second before disappearing. The launcher doesn't Start *at all* 
	
Cause: Windows UAC is preventing running of this program. 
	
Work Around:
1) Open a Power shell windows as a administrator from the search bar and type **Set-ExecutionPolicy Bypass** 
		Answering yes to any questions which follow
		
2) if 1) doesn't work - navigate to the "\_shortcut" folder and start one of the batch files matching your preferred graphics settings

Note: If the launcher does start but crashes after clicking "play" please see this FAQ entry [Game Hard CTD on Splashscreen](#game-hard-CTD-on-SplashScreen)

---
### Can I see a list of Known issues?

Sure - Here's a [link](https://docs.google.com/document/d/10jxUuBhmnLne5e4lb7ifAz9rByrTy_wEOpojmItyScM/preview)

---
### What do the presets mean?

High   - Intended for top end PC, grass is visible from maximum distance Skyrim is capable of drawing (equivalent to Ultra)

Medium - Intended for Mid-range PC's - grass is visible from approx 10 meters(equivalent to medium-high)

Low    - Intended for minimum specification PC - grass is only drawn literally a meter away - may have odd visual effects during heavy snow 

---
## **Install Questions**

### How do i setup a steam library outside of program files

The Wabbajack team has a handy utility to help you do that [here](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide)

---

### I’m missing master for HighResTexturePack01-03 or My game CTD after Skyrim Logo

If you are experiencing a missing master for HighResTexturePack01-03 the simplest fix is to download and enable the High Res DLC from https://store.steampowered.com/app/202485/Skyrim_High_Resolution_Texture_Pack_Free_DLC/

Alternatively, you can re-run the Reqtificator to generate a new Requiem For The Indifferent.esp (RFTI) without the High Res DLC as a master. This will be fixed in the next release.

If you have issues viewing the DL, try this work around https://www.reddit.com/r/ultimateskyrim/comments/galfjk/high_res_texture_pack_info/

---

### Game doesn't boot when launching SKSE / Cannot Start SKSE_Loader Error

Ensure the following:

1. Check that your Anti-virus is not flagging SKSE or any Skyrim related files (best Solution is to add Anti-virus exceptions to  the Ultimate Skyrim & Skyrim folders

2. Make sure you content folder contains usvfs_proxy_x64.exe & usvfs_proxy_x86.exe If these files are missing its likely your anti-virus has moved them to the virus vault.

3. Restore Missing files from Mod Organizer Zip file in your Ultimate Skyrim\download directory if cannot find in virus vault

---

### Game Hard CTD on Splashscreen

Note: You may get a error messages about missing d3dx9_43.dll.

Attempt starting Skyrim from steam - if this crashes as well then

1. Download DirectX End-User Runtimes from [Here](https://web.archive.org/web/20190616115008/https://download.microsoft.com/download/8/4/A/84A35BF1-DAFE-4AE8-82AF-AD2AE20B6B14/directx_Jun2010_redist.exe) or [here](https://download.cnet.com/Microsoft-DirectX-Redistributable-June-2010/3000-2121_4-10176490.html) Note: This will give you a zip file disguised as a EXE - not the actual installer itself
2. Unpack the downloaded file into a directory (E.g C:\directX\)
3. Open the directory and run DXSetup.exe. Follow on-screen instructions.
4. (optional but recommended) Reboot your PC.

If Skyrim Launches from steam 

1. Go in the Windows control panel, Region. 	
2. Click "Additional settings..." at the bottom, then "Reset" in the window that opens.

Other things which can cause this issue:-
* ASUS GPU TweakII, Xtrem tuner or MSI afterburner running at the same time as Skyrim
* You have moved your "my documents" folder to a different hard drive - SKSE requires this to be on your System drive.
* You have overlay's running (Steam, Discord, geforce experience, overwolf ect)

---

### Skyrim has failed to allocate memory! or Possibly running out of memory

If your game CTDs with an error from Crash Fixes saying "Skyrim has failed to allocate memory! Possibly running out of memory...", or it crashes during/after the character creation screen, the most likely cause is a bad ENB installation.

Open  “enblocal.ini” in your Skyrfilm folder and then configure it according to this

![yfBDnJI](https://github.com/Wildlander-mod/wildlander-mod.github.io/assets/26418143/464543de-67f6-4898-bd10-d943a2efdbe1)

---

## **Customization Questions**
### Can someone help with my load order?

The Ultimate Skyrim Support Team cannot assist with this issue as there are too many variables. 

Do not use L.O.O.T or rearrange Ultimate Skyrim’s default mods unless a guide from one of us specifically tells you to!


**If you have broken you load order and want to get back to the original**
* Close Mod Organiser
* If you have profile specific saves - Back these up first (they will be in <install path>\content\profiles\profile you play\saves).
* delete everything from <install path>\content\profiles\

Download the appropriate zip file for the version of Ultsky you currently have installed:-	

* For 4.0.7 Installs https://wiki.wildlandermod.com/Assets/Downloads/profiles.rar
* For 4.1   Installs https://wiki.wildlandermod.com/Assets/Downloads/4.1_profiles.rar 
* for 4.2   Installs https://wiki.wildlandermod.com/Assets/Downloads/4.2_profiles.rar
* for 4.3   Installs https://wiki.wildlandermod.com/Assets/Downloads/4.3_profiles.zip
* Unpack the contents of the correct zip file for your installation into <install path>\content\profiles\.

If you have added additional Mods - you will need to re-enable & reorganize your load order. 

Finally if you had profile specific saves - recreated the saves directory and restore your saves from your backup.

---

### Mod X has been updated, can I install that?

No, For stability reasons - only the versions installed by Wabbajack are supported.

---

### Can I remove/disable mod X?

Many mods have a Mod Configuration Menu (MCM) where they can be turned off. Also, some mods are considered optional, so they can be disabled or uninstalled in Mod Organizer. If you remove an optional mod that has an esp plugin, you will need to run the Reqtificator and possibly Automatic Variants patcher. 

---

### Can I Add Additional mods?

For a list of known mods which have Issues/Incompatibilities/ please click [here](https://wiki.wildlandermod.com/16OtherResources/UltskyModdingGuide/#known-mod-issuesincompatibilities)

Before you begin modding Please read the [basics](https://wiki.wildlandermod.com/16OtherResources/UltskyModdingGuide/#ultimate-skyrim-modding-basics) which contains the rules for modding in ultsky and are slightly different to other modlists you might have tried. The most important rule is

▶️ **YOU CANT USE LOOT**  ◀️

The support Team has put together a set of guides for adding popularly requested additional mods.

Please visit [this page](https://wiki.wildlandermod.com/16OtherResources/UltskyModdingGuide/#guides-list) for install guides or the Wildlander discord (Ultsky-customization channel) advice for other type of mods.

---

### Does This mod pack Support other languages?

No and if you try then SKSE crashes from Mod Organizer. You will need to install English Skyrim to play this mod pack.

---

### Can I backup and restore Ultimate Skyrim

Yes, please follow this [guide](https://github.com/Wildlander-mod/Support/blob/master/Docs/Backup.md)


---
### I want to setup rodericktech guide for fancy graphics - where are the patcher instructions.

Reqtificator is located [here](#how-do-i-install-the-reqtificator)

Other Patchers(AV, Dyndolod ect) are located [here](https://wiki.wildlandermod.com/16OtherResources/UltskyPatchers/)

---

### My PC can't handle the ENB - Can I reduce the Settings?

If you prefer to keep Dylan's lighting preferences - then open up ENBseries.ini in you Steam Skyrim folder and change the effects section to match the following

![image of Low ENB Settings](https://media.discordapp.net/attachments/348579495537803274/763697916992552970/unknown.png)

If on the other hand you want absolute best performance, but retaining the ENB weather & lighting effects you can switch your ENBseries.ini in your Steam Skyrim folder with this one [enbseries ini](https://cdn.discordapp.com/attachments/785284178282676234/785284699240792084/enbseries.ini)  

---

### It's too dark at night, can I make it brighter?

for regular vision

Open ENB GUI in game with shift+enter. In the enbseries window, find the weather toggle and turn that on. In the weather pane, find the Environment section, find Point lighting. There are several settings you can adjust here. Just play around with them to see how everything works and find what you like. If you screw something up and forget the default value or just want to revert to your previous saved settings, just hit load settings in the enblocal window. 

When you want to save, hit save then apply in the enblocal window.

For Nighteye Settings
[ENNE NightEye Settings](https://www.reddit.com/r/ultimateskyrim/comments/bpk1js/adjusting_night_eyeeene_for_better_visibility/)

---

### My PC Can't handle the ENB Graphics even on low settings - Can I remove it?

Skyrim can't handle modern PC's RAM capacity So if you PC has more than 4GB you cannot disable the ENB entirely - so the most you are able to do is deactivate the ENB graphics and just use the memory boost (ENBboost) aspects.

Delete ENBseries folder and ENBseries.ini from your Steam Skyrim folder

1) Open Content\ModOrganiser.exe
2) Select the graphics profile you play from the profiles drop down
3) find on the left side Snowfall weathers and untick that
4) find ultimate skyrim - snowfall weathers.esp on the right side and untick that too
5) Setup and run the Reqtificator as per [Instructions](#How-do-i-Install-the-Reqtificator)
6) Open Skyrim\Enblocal.ini, Change UsePatchSpeedhackWithoutGraphics to true.

---

## **Reqtificator Questions**


### There was no consistency file found
![unnamed](https://github.com/Wildlander-mod/wildlander-mod.github.io/assets/26418143/3c65ee1a-55dd-4e61-92d5-d891c8bf0c3f)


Select “Yes, this is a new game.”

---

### Automatically allocating memory failed

![unnamed](https://github.com/Wildlander-mod/wildlander-mod.github.io/assets/26418143/4b98e1ad-f986-4e8f-abb5-8c36f955059f)


Your binary path for java is wrong. The Reqtificator error message tells you that you're using 32-bit java instead of 64. Check your paths in _Step 5_[ https://requiem.atlassian.net/wiki/spaces/RS/pages/691470460/Installing+Requiem+with+Mod+Organizer+2+version+3.2.0+and+older](https://requiem.atlassian.net/wiki/spaces/RS/pages/691470460/Installing+Requiem+with+Mod+Organizer+2+version+3.2.0+and+older)

---

### It says I am using more than 100 plugins

![unnamed](https://github.com/Wildlander-mod/wildlander-mod.github.io/assets/26418143/dc7035a8-d102-4a53-93b0-922cce872e50)


Select ignore from now on

---

### The Reqtificator won't start. When I press "Run", MO2 locks up, then unlocks and nothing happens; or MO2 returns a "Directory name is invalid" error.

In most cases this is due to a typo in the folder path for the Requiem Skyproc patcher. The path should be: **\<path to your Skyrim installation>\Data\SkyProc Patchers\Requiem**. Many users omit the 's' at the end of "SkyProc Patchers" when creating the folder. Also confirm that the "Start in" path in your MO2 Reqtificator configuration matches the path.

---

## **MCM Questions**

### What does the MCM guide mean about template saves?

There is unfortunately no way to Copy MCM settings over to a new character for every mod. 

The closest thing is creating a "template save" by configuring the bulk of the MCM's. then loading this template save everytime you want to create a new character. You will then only need to do the "post-Start" MCM setups (approx the last 2 pages)

A template save will be the save game you make _before_ clicking on _Begin My Adventure_ in the Ultimate Skyrim MCM menu, you will want to do this so next time you start a new character you won’t have to re-configure everything before the Ultimate Skyrim MCM!

Disclaimer

*Certain elements of a game are *baked* into Skyrim the *exact moment* Start New Game is selected. These types of elements are; Locations of certain items*

---
### iNeeds MCM page is blank Or Requiem Cannot be added to a existing save.

This happens when you start MCM config before the mod has finished initialising - indicated by scrolling messages in the top left of your screen. 

There is no way to recover you game once this occurs.

1) You will need to close & re-open Skyrim, to remove partially loaded scripts from your session.
2) Start a new game
3) Wait for **all** messages in the top left to disappear
4) Start MCM setup again.

----


## **Gameplay Questions**

---
### Why are auto-saves disabled or quicksaves not recommended for use in Ultsky

The problem in a heavily modded set up is that it has a ton of script heavy mods. Sometimes a script will get paused for saving, and that script won't be able to recover properly from it's paused state. This leads to a corrupted save. Another possibility is that your computer is already under so much strain from the scripts that the save function can actually cause a ctd when trying to save, usually during some script-intensive moment.

The point being that not using auto-save can help with avoiding ctds (if you've been experiencing them on loading Screens) and hence corrupted save files when you try to load one after a CTD. In addition Auto-saves increase cell loading times by 500%, so its preferable to manually save once inside of a cell, rather than have it integrated into the loading screen. 

Quicksaves are fine as long as you know when to save (i.e. during low intensity moments, giving plenty of time for your crazy mod scripts to finish running) and not while hiding behind a pillar in stealth trying to avoid 50 bandits whom you just woke. 

Auto/Quicksaves are not bad intrinsically (in and of themselves), it's that there are an insufficient number of them if something goes wrong, leading to the possibility of many lost hours of game-play progress. You would be forced to use a previous 'hard save.'.

TL;DR  Auto/Quicksaves are ok, but timing is what determines if they're safe or more likely to corrupt.  Having multiple saves to use limits the amount of play lost to script-death.

Instead Practice Safe Hard saves:-
> When you load your save file, wait at least a minute before saving again. Some scripts will break if you save too soon after loading.
>  
> Avoid saving during combat or other conditions of heavy script load. 
>
> Never save more than once a minute.
>
> Never save within 30 seconds of entering a building / cell / dungeon.

---

### My Keyboard isnt working

Normally occurs if you have ran special Edition version of skyrim prior to loading Ultimate skyrim. Special edition doesnt release all of the files Legendary edition needs to run so disables the keyboard.

1) Some users report that closing and reopening steam itself is enough to make it work
2) Reboot your PC.

---

### My Compass has disappeared!

This is intentional. Immersive HUD hides this functionality by default. To make the compass _temporarily_ visible again press the 'N' key.

-   To make it permanently visible, change the MCM setting in Immersive HUD > Compass Activation > Key Press Toggles.

---

### Why can't I select the first crafting perk?

You need a book called The Craftsman’s Manual in your inventory. It can be purchased from most blacksmiths. Most of the Requiem crafting perks require their own books, some of which can be bought while others must be found in the world.

---

### Why Can't I Run or Why is my stamina going down for no reason?

Requiem applies a stamina draining effect when you run, and when you wear armor without the first perk in the heavy/evasion armor tree. Running is the normal speed you move at if you aren’t sprinting or specifically holding down the “walk” button. To combat this, make sure to buy food with a “Regenerate 1 stamina per second for X seconds” effect and keep that buff up at all times.

**NO YOU CANNOT DISABLE IT, PLEASE DON'T ASK!**

---

### Why can't I get a blessing at a shrine?

Requiem's Gods are unforgiving of crime. Too much crime and they will no longer bless you or heal you!

---
### Why arent I healing?

Requiem disables passive health regeneration, you will need to obtain a healing poultice or a potion to regenerate health. 

---
### My character is glowing ugly orange patches at night.

This is how the ENB expresses the dirt shader - Take a bath!

---

### Error: Incompatible menu file(Map.swf) when opening the map.

You missed an MCM setting in SkyUI! Open SkyUI MCM Menu > Advanced > uncheck 'Map menu' in  SWF Version Checking section.

---

### My vision is all Blurry/Messed up!

 1) This can happen if you eat too many alchemy ingredients too quickly. Find and eat a Nirnroot to remove the effect.
 2) Check you active effects, you might have picked up a disease and require a potion of cleansing.

---

### The screen randomly went dark shortly after I entered &lt;insert name here &gt;.

This is caused by Darker Dungeons. If you would like to disable this option, open up Darker Dungeons MCM > General Configuration > _untick_ Do Fadeout On Dungeon Entry.

---
### Lights are Flickering on and off

Most noticabled in Breezehome but can happen everywhere.

This is caused by Skyrim's engine limitation of 4 lightsources in a area. when you look in a area with more than 4 lightsurces they alternate/cycle and turn on and off.

Only resolution is to use Cobb Positioner's to identify lightsources, and delete extra's.

---

### I tried to learn a spell from a Tome - the book disappeared but I still don't know it

You missed loading SV Mods Preset during your Post-Start MCM Setup. To fix navigate to SV’s MCM menu > Save/Load Preset > FISS > Click ‘Load Preset’.

---

### Why does the NPC dialogue cut out when talking to Aela?

Enhanced Skyrim Factions - The Companions Guild adds new conversation options to NPCs that aren’t voiced. Other NPCs have the same behavior.

---

### My game has no grass or has very little grass

Ensure the following are set in Content\Profiles\<Profile you play>\:

1. Make sure that skyrim.ini has the settings `bAllowCreateGrass`, `bAllowLoadGrass`, and `bDrawShaderGrass` set to 1

2. Decrease the `iMinGrassSize=` setting, this will increase grass density(default Skyrim has a setting of 20, 60 is the recommended if you are using a plugin like Verdant)

3. Change `iMaxGrassTypesPerTexure=` Default is 5 and max is 15. (note: the misspelling of texture is a mistake on Bethesda's and should be replicated)

---

### Why is everything so expensive in shops?

You’re Naked - Put some clothes on ya filthy animal!

---

### I am getting a lot of stutter / CTD / Low FPS?

*Ultimate Skyrim will never go above 60 FPS due to limitations of skyrim's engine. if you think 60fps is low - too bad. It cannot run any higher.*

Never have Task manager open while running Skyrim (not even minimized to task bar). If your CTD are occurring during a loading screen - this is your cause.

Make sure that you haven't included a comma in the "VideoMemorySizeMb" field in ENBlocal.ini

Make sure you haven't changed "FPSLimit" field in the limiter section in ENBlocal.ini (default is 59.900002)

Try turning off vsync & g-sync for Skyrim(TESV.exe) in the Graphics Card Settings. 

Close down any background programs which maybe injecting into direct X (graphics card software such as geforce experience and MSI afterburn are two culprits)

Check your background processes. Skyrim is highly reliant on CPU - Core 0, so if your CPU is busy with other tasks it might be causing the stutters

Run Bmxfreestyle’s Stability Guide and follow the recommended tweaks (pinned in #ultsky-support).

[https://discordapp.com/channels/344256550640287755/348579495537803274/729035407282667662](https://discordapp.com/channels/344256550640287755/348579495537803274/729035407282667662)

Once you have checked all of those you can apply the following tweaks.

1. Attempt to disable border less window in <ultimate Skyrim>\content\mods\UltSky (Version Number) Core Files\SKSE\Plugins\OneTweak.ini. If you want to play Full-screen after doing this instead of windowed you will also need to change BFullScreen to 1 in content\profiles\UltSky (preset you play)\Skyrimpref.ini.  (This makes your computer focuses on the game and give a good +10 fps boost, at the expense of speedy alt-tabs)
	
1. Lower your Graphics preset, or adjust content\profiles\UltSky (preset you play)\Skyrimpref.ini	reduce the iShadowMapResolution (can be changed to 1024 or 512), fShadowDistance and fGrassMaxStartFadeDistance.
	
1. [Lower]( https://wiki.wildlandermod.com/16OtherResources/UltSkyFAQ/#my-pc-cant-handle-the-enb---can-i-reduce-the-settings) or [uninstall]( https://wiki.wildlandermod.com/16OtherResources/UltSkyFAQ/#my-pc-cant-handle-the-enb-graphics-even-on-low-settings---can-i-remove-it) the ENB	

---

### When I equip my Lantern/Backpack I get a pouch/book/holder/carpet appearing in my inventory

This is a bug - cause unknown. Although there is no permanent fix, you can _possibly_ solve it by either dropping and buying a new item OR by dropping your item and consoling one in.

---

### When I equip my Belt items it doesn’t ask me which slot I want to put it in

Drop the item, and pick it back up then it will ask you where you would like to place it.

---

### When I drop items on the ground, they sometimes vanish

1. This seems to happen occasionally when dropping items in 1st person view. Try switching to 3rd person before dropping them.

2. if the items are related to one of the following mods; Campfire, Wearable Lanterns, or Bandoleers - Bags and Pouches, this is likely due to a corrupted ID (BAD EDITOR ID when you do player.showinventory)

---

### My Lantern/Tent is asking me where I’d like it equipped

This is due to a bad ID, breaking down your lantern and re-crafting it in the crafting ledger usually fixes your lantern, if you have the craftsman perk it's advisable to make your own, if you don't just purchase a new tent from any vendor.

---

### How do I re-enable menus pausing?

SkyrimSouls.ini controls which functions pause the game. You can edit the INI file from Mod Organiser. Right click the `Ultimate Skyrim 4.0.6 hf2`, `Ultimate Skyrim 4.0.7 core files` or  `Ultimate Skyrim 4.1.0 core files` or  `Ultimate Skyrim 4.2.0 core files` mod in the left pane -> Information -> ini files tab.

---

### My character's animations are stuck.
This is a vanilla Skyrim bug, exacerbated by the scripted mods in Ultimate Skyrim. If jumping doesn’t fix the animation, try the following console commands:

	Pushactoraway 14 1
	SetPlayerAIDriven 0

---

### I keep hearing strange noises around me or objects floating around

This is usually a symptom of a known physics engine limitation, causing game instability at frame-rates higher than 60 FPS.  The easiest workaround is to limit the frame-rate to 60 FPS, either in the ENB configuration (Shift+Enter opens it in-game), or in the GPU software.

---

### If you have Clouds on your Paper world map

This is a Known issue - Please visit the Official discord #ultsky-FAQ channel for the list of known issues and correction instructions
	
---
### My Character Spawned Underwater

If you load into the game (or start a new character) and your character is underwater while outside, usually near either Whiterun or Markarth's bridges. The Fix is to Enter a nearby building then exit again to force skyrim to re-load the cell.


----
### Why Can't I Fast Travel

Requiem disables Fast travel. There are multiple methods of moving around the map quickly without using this - There are boats near most large area of water, and Carriage drivers at the cities.

----
### My game freezes during loading screens.

The game may appear frozen or have a unusually long loading time, but it's usually still loading in the background. This is caused by OneTweak's Windowless Bordered mode. 

* Please make sure that Windows Task manager is not running.
* Dont Alt-tab out of loading screens.
* Disable Save on wait and Save on travel and switch to using manual saves if problem exists while moving between cells in-game.

Can also be caused by

* Your PC being below the minimum requirements to play the pack as shown on the install Readme. You can try removing the ENB [using](  https://wiki.wildlandermod.com/16OtherResources/UltSkyFAQ/#my-pc-cant-handle-the-enb-graphics-even-on-low-settings---can-i-remove-it).	
* Ultimate Skyrim folders(or subfolders) being read-only.
* Ultimate skyrim being on a different drive to skyrim - Only resolution to this is to move Ultimate skyrim to same hard drive.
* Ultimate skyrim being installed inside of program files - Move the ultimate skyrim to a folder outside of program files.
* Additional mods in skyrim\data folder from previous modding or workshop subscriptions are causing a conflict.
* Conflict between 5000 & 6000 series AMD drivers and the ENB - only resolution to this is to either roll back until you find working AMD drivers or disable ENB graphics using [step 6 of](  https://wiki.wildlandermod.com/16OtherResources/UltSkyFAQ/#my-pc-cant-handle-the-enb-graphics-even-on-low-settings---can-i-remove-it) until a working driver is available.
* A Corrupt Skyrim installation (to check, launch skyrim from steam and see if it crashes on loading screen)
* Antivirus real-time scanning your Skyrim\ultimate skyrim folders - add ultimate skyrim and skyrim folders to your exceptions. 
* [Direct X](#game-hard-CTD-on-SplashScreen) and/or [C++](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) installations are broken (You’ll need both the 32-bit and the 64-bit versions of C++.)
* You have lost permissions to write to "my documents\My Games\Skyrim" or ultimate skyrim install folder
* Onedrive and/or dropbox is Syncing your "my documents\My Games\Skyrim" or ultimate skyrim install folder 
* Can be caused by a corrupt save, you can try using [Savetool.exe](https://www.nexusmods.com/skyrim/mods/52363/?) to see if you can load your save if this also fails then you will need to revert to a previous save or start a new game.


----
### How do I change the difficulty?

The in-game difficulty sliders do not work with Requiem. Use the Damage Dealt/Taken values in the Requiem MCM instead. The recommended setting for both sliders is 100%. Requiem increases the difficulty of the game significantly, so if you're having a hard time doing anything, take a look at the [Beginner Guide for New Requiem Players](https://www.reddit.com/r/skyrimrequiem/comments/1w5cej/surviving_the_first_few_hours_in_requiem_or/).

----
### I contracted Sanguinare Vampiris and now I can't sleep!

This is a Minor Arcana change that prevents weak characters from acquiring Vampirism. You must survive for 3 days while Sanguinare Vampiris slowly drains health and negates natural healing, at which point you will become a Vampire.

----
### My Grass/Tree's in distance are shimmering/flickering

This is caused by the ENB when used on some graphics cards. 

You can choose to add a "max FPS limit" on your graphics card for "TESV.exe" to "59" as this reducing flickering on some cards (especially if the moniter connected to the card has a high refresh rate)

The following guide has also shown improvement when both the step guide, and U/seq Comments are followed.

https://www.reddit.com/r/ultimateskyrim/comments/gfdg6l/antialiasing_is_b_a_d/
	
The original site has long gone - but a mirror of the injector is available here https://www.softpedia.com/get/Tweak/Video-Tweak/injectSMAA.shtml#download	

Note: this is the only 'fix' support are aware of at this time and if it does not work for you, we won't be able to assist you further

---
### Eorland Graymane wont temper/craft stuff for me

Eorland Graymane is the best smith in the game, and as such reserves his services for members of the Circle for the companions.

Note: you must be at least at the stage of "Kill the werewolf hunters" for the Quest "The silver hand"

---

### How Do I Enable Permadeath
In short - You cant. Permadeath mod Ashes was removed from the build of ultimate skyrim back in september when 4.0.7 was released.

Instead of a 'permadeath mod' the player, upon dying is presented with the Requiem death dialog telling you to load a save. If you wish to be permadeath, simply load your template save at this point and start a new character (manually deleting all of the saves for your dead character)

---

## **4.0.6 Issues**


### I have this really weird red/green/brown/black graphical issue on the bottom half of my screen

4.0.6 Issue

![unnamed](https://wiki.wildlandermod.com/Assets/UltskyGlitch.webp)

You probably messed up installing the custom INI files. Make sure you are installing Skyrim.ini and SkyrimPrefs.ini in the `\Ultimate Skyrim 4.0.x\profiles\Ultimate Skyrim 4.0.x (Full)` folder!

---

### My rain splashes are purple/pink!

4.0.6 Issue

You need a patch! ([US 406 HF2] Fix for purple/pink rain splashes (Wonders of Weather). Install with MO2 and keep at the end of the mod list on the left side (no esp). Fix is on [Official UltSy discord](https://discordapp.com/invite/8VkDrfq) in #ultsky-bug-submission channel (incase link doesn't work).

[https://discordapp.com/channels/344256550640287755/566419501613318154/680786963615186946](https://discordapp.com/channels/344256550640287755/566419501613318154/680786963615186946)

---

### Why am I not leveling up!

4.0.6 Issue

You only get experience while sleeping - Take a nap!

---

### My character is invincible - I get to zero health but don't die!

4.0.6 Issue

You need a patch! `[US 406 HF2] Ashes 0.02 patch v0.6.`  Fix is on [Official UltSy discord](https://discordapp.com/invite/8VkDrfq) in #ultsky-bug-submission channel (incase below link doesn't work).

[https://discordapp.com/channels/344256550640287755/566419501613318154/679539347854327829](https://discordapp.com/channels/344256550640287755/566419501613318154/679539347854327829)

---

### I'm trying to load my template save and it says my character is dead.

4.0.6 Issue

This happens when you name your character the default name "Adventurer" and are killed by permadeath. To fix delete the .dead file in your `steamapps\common\Skyrim` folder and you will be able to load your save.

---

### My Character takes off of his/her clothes off when swimming

4.0.6 Issue

To stop this from happening, open Bathing in Skyrim MCM > Player Animations and _untick_ everything in the sections “Undress Before Bathing - Standard” and “Undress Before Bathing - Extended”

---

### Why isn’t my compass showing undiscovered locations?

iCompass hides the locations by default. To restore your compass to vanilla setting, _uninstall by unchecking_ iCompass in MO2 and rerun Reqtificator.

_Please note, installing or uninstalling mods during a playthrough may break your game and is not recommended_


## **Questing Questions**

### How do I start the main quest?

Kill a dragon. Make sure you’re set as Dragonborn in the Ultimate Skyrim MCM.

---

### Why can't I obtain the dragonstone?

This quest is auto completed when you kill a dragon.

---

### How Do I Become Thane of Whiterun

There is a new way of becoming a thane of Whiterun. Complete The Blessings of Nature quest(Danica by the Gildrergreen tree to start) and talk to Jarl Balgruuf when the Gildergreen tree is repaired\the sappling blooms. He'll thank you and allow you to buy the Breezehome, and the standard thaneship quest (help the people of the hold and buy a house) will be available.

---

### I can’t start the Thieves Guild through Brynjolf.

**Thieves Guild Requirements** is included in the list, which requires a certain amount of pockets picked/items stolen.

---

### How do I start the Dragonborn questline?

Dragonborn content is available after completing "A Blade in the Dark" during the Main Quest.

---

### How do I start the Undeath questline?

Undeath content is available after level 30. A quest will appear in your journal with further instructions.

---
