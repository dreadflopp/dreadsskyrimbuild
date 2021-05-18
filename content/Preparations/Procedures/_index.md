+++
title = "Procedures"
weight = 10
description = "Descriptions and instructions on common modding procedures."
+++

###### Common modding procedures

## Using Mod Organizer 2

This guide uses Mod Organizer 2 (MO2), but you may use whichever mod manager you are comfortable with as long as you know how to properly use it. To learn how to use MO2, watch the [tutorial videos by Gamerpoet](https://www.youtube.com/playlist?list=PLlN8weLk86Xh3ue76x2ibqtmMramwQmHB) or read the [STEP guide for Mod Organizer 2](https://stepmodifications.org/wiki/Guide:Mod_Organizer).

## Sorting with LOOT

At any time during the mod installation process LOOT should be used to sort plugin load order before running the game. This is necessary to ensure proper plugin priority (load order), which can have a dramatic impact on the game. Users not running the game during the mod installation step of the Guide can wait to sort after this step is complete. To sort with LOOT:

1. Launch LOOT via Mod Organizer 2 from the executables drop-down menu.
1. Click the “Sort” button at the top of the LOOT window.
1. Examine the resulting order carefully and look for any alerts or warnings and take  note of these. Ignore warnings about patches being available. Patches are provided by this guide.
1. Click the “Apply” button, which has replaced the Sort button at the top.
1. Close LOOT.

## Standard cleaning procedure

Some mods, as well as the official vanilla game, contains plugins (.esp-files) or master plugins (.esm-files) that are dirty. LOOT warns you about such plugins. Clean all plugins that LOOT prompts you to clean. To clean a plugin:

1. Run xEdit64 Quick Auto Clean through Mod Organizer 2.
1. Select the plugin being cleaned (i.e., Update.esm, Dawnguard.esm, etc).
1. xEdit will now automatically clean the *Identical to master* and *deleted* records from the selected mod.
1. Once xEdit is done cleaning, click the X in upper right of the program window to close the program.

## Converting plugins

Many plugins made for classic Skyrim works without issues with Skyrim Special Edition but the plugin form format (form 43) should be updated to Skyrim SE's form format (form 44). To achieve this, simply open the plugin in the Creation Kit and re-save it.

Whenever the guide prompts you to convert a plugin, follow these instructions:

1. Run the Creation Kit through Mod Organizer 2.
1. Select the *File* menu and choose *Data...*
1. Find the plugin to be converted and select *Set as Active File*.
1. Note the Parent Masters listed and ensure they are checked (double-click the plugin listing to check it).
1. Click *OK* and allow the Creation Kit to load the files.
1. Once complete, simply save the plug (icon on toolbar or Save from the File menu).
1. Close the Creation Kit.

Use SSEEdit to check that no errors were introduced in the plugin during the conversion:

1. Run SSEEdit through Mod Organizer 2
1. Right-click in the plugin pane and choose Select *None*.
1. Select the plugin being checked and click *OK*
1. Allow SSEEdit to load and process all plugins.
1. Right-click on the last plugin in the left pane (it should be the new plugin), and select Check for Errors.
    * The check should come back reading, *"All done!"*. If there are errors reported, reinstall the mod and redo the conversion.
1. Right-click on the plugin again and choose, *Sort Masters*.
1. Close xEdit and be sure the plugin is checked in the saving prompt.
