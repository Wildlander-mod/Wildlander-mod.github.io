---
layout: default
title: How Do I edit the UI?
has_toc: false
has_children: false

---


The Main UI elements are controlled by a bunch of INI files

## For the main UI elements and positions

game-files\mods\Wildlander\interface\skyhud\Skyhud.txt

The mod used is SkyHUD. This doesn't have a in game interface, so to edit the UI you need to open the above file. makes you changes and then save and load the game to check the result.

While i find the INI is fairly self explanatory, Should you need further help that that the mod page download for SKyhud has a reference manual you can download in the Miscellaneous files section <https://www.nexusmods.com/skyrimspecialedition/mods/463?tab=files>. 

## for the contextual crosshair 

game-files\mods\Wildlander\SKSE\Plugins\ContextualCrosshair.ini

This mod controlls the cursor. If you want a "always on" cursor then you can disable the contextual crosshair mod in mod organiser.

## to edit the Item card on 16:10 moniters so it doesnt "clip" (set bEnableItemCardResize=0 )

game-files\mods\moreHUD Inventory Edition\SKSE\Plugins\AHZmoreHUDInventory.ini

You may also need to edit SkyHUD for widget positions.

## The Weapons display UI widget

This is controlled in game via the iEquip program. You will need to rebind "edit mode" to a unused key.

Note: this function is known to cause CTD's unless you temporarily disable ConsoleUtil in MO2. Some users report that entering the MCM menu for iEquip and turn time dilation down to zero also prevents the CTD. regardless of which option you choose, you will need to reset either consoleutil or time dialation back to defaults after making your changes.

## Frostfall Meters

This is controlled by a Ingame MCM, to navigate to the Frostfall MCM 
1. Escape menu
2. Mod configuration
3. Frostfall

Before making any changes it is recommended that you switch the Frostfall profile, otherwise you'll overwrite Wildlander-defaults ("ULTSKY010-WORKING" and can't easily switch back) To do this,  Under "Profiles" submenu select another slot (#2 to #10). See MCM "About Settings Profile" for further details. And NEVER use "DEFAULT CURRENT PROFILE!"

To edit the meters, select “Meters” submenu. 
* You can change the Display Mode from always-on to contextual. 
* Under "Advanced settings" you can customize position, scale, color and opacity."


