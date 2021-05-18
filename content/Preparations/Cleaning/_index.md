+++
title = "Cleaning"
weight = 20
description = "Instructions on how to clean the vanilla files."
+++

###### Cleaning vanilla master files

To remove redundancy and errors in Skyrim's master plugins, it is recommended they be cleaned with SSEEdit before modding begins. This ensures maximum stability and compatibility within the modding experience. This section of the guide walks you through three steps; creating an empty mod in MO2 for the cleaned files, cleaning the files and lastly moving the cleaned files to the created empty mod.

## Create an empty mod

1. On the MO window, click the Open list options button at the top of the left pane, next to the profile selection drop-down.
1. Choose Create empty mod, name it *Cleaned Vanilla Masters*, and click OK.

## Clean the masters

Vanilla masters should be cleaned in the following order:

1. Update.esm
1. Dawnguard.esm
1. Hearthfires.esm
1. Dragonborn.esm 

Follow the standard cleaning procedures to clean Update.esm, followed by Dawnguard.esm. Once Dawnguard is cleaned, complete the manual cleaning below:

1. Run SSEEdit from MO2.
1. At the prompt, double-click on Dawnguard.esm.
1. Once loaded, type in 00016BCF in the FormID field (above the mod list) and hit **Enter/Return**.
1. In the right pane, find the **XEZN - Encounter Zone** record.
1. In the Dawnguard.esm column, right-click on the *RiftenRatwayZone \[ECZN:0009FBB9\]* entry and select Remove.
    - If a prompt appears select Yes for each of these removals. 
1. In the FormID field again, type in 0001FA4C and hit Enter/Return.
1. On the Dawnguard.esm column, right-lick on the Dawnguard.esm header and select Remove.
1. In the FormID field again, type in 0006C3B6 and hit Enter/Return.
1. On the Dawnguard.esm column, right-lick on the Dawnguard.esm header and select Remove.
1. Now close SSEEdit, ensuring Dawnguard.esm is checked on the prompt.

Once Dawnguard's manual cleaning is complete, follow the standard cleaning procedures to clean Hearthfires.esm, and then last, Dragonborn.esm.

## Moving the cleaned files

After the vanilla master files are cleaned, users should move them to their created mod listing in MO2 and restore the original files. This prevents users from having to re-clean the files after verifying their cache in Steam. To do this, complete the following:

1. In a new window, open the Skyrim Special Edition Data directory (e.g. ..\Modding\Steam\steamapps\common\Skyrim Special Edition\Data)
1. Drag and drop (or copy and paste) the four cleaned master files from Data to the *Cleaned Vanilla Masters* folder.
1. In the SSEEdit Backups folder, rename the files to their original names (e.g. *Update.esm*, etc).
    * If there are multiple copies of any of the files, use the one with the earliest timestamp. 
1. Drag and drop the renamed files from the xEdit Backups folder to the Data directory and choose to overwrite/replace, if asked.
1. Close the explorer windows.
1. Drag and drop the new Cleaned Vanilla Masters mod listing in the left pane directly below DLC: Dragonborn.esm.

At this point, the Bethesda masters should be cleaned and the mod list order should reflect: 

1. DLC: Dawnguard.esm
1. DLC: HearthFires.esm
1. DLC: Dragonborn.esm
1. Cleaned Vanilla Masters