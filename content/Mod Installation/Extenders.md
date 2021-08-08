+++
title = "Extenders"
weight = 10
+++

### SKSE64
{{% button href="http://www.nexusmods.com/skyrimspecialedition/mods/30379" icon="fas fa-download" icon-position="right" %}}Download{{% /button %}}

**Root Files Installation**

1. Download the most current archive for Skyrim SE.
1. Open the downloaded archive and extract the following files to the Skyrim Special Edition folder: (..\Steam\steamapps\common\Skyrim Special Edition\) 
	* skse64_X_X_X.dll
	* skse64_loader.exe
	* skse64_steam_loader.dll 

**Data Files Installation**

1. Open MO2 and right-click on the mod list.
1. Hover over All Mods and select Create empty mod.
1. Type in SKSE64, or anything similar.
1. Hold down the Ctrl key and double-click on the newly created mod in the mod list.
1. Keep this folder open for the next two steps below. 

**INI File**

1. In the new Explorer window, create a new folder named SKSE
1. Open that folder and create a new file named SKSE.ini
1. Open the new file and copy and paste the code in the box below
1. Save and close the file.

```
[Display]
iTintTextureResolution=2048

[General]
ClearInvalidRegistrations=1
```

**Scripts**

1. From the archive downloaded above, open the Data folder (..\skse64_X_X_X\Data\)
1. Extract the Scripts folder to the mod's folder.

Once complete, the SKSE mod's folder structure should look like this:

![Settings](/dreadsskyrimbuild/images/SKSEinMO.jpg)

### .NET Script Framework
{{% button href="http://www.nexusmods.com/skyrimspecialedition/mods/21294" icon="fas fa-download" icon-position="right" %}}Download{{% /button %}}

### No Grass In Objects
{{% button href="http://www.nexusmods.com/skyrimspecialedition/mods/42161" icon="fas fa-download" icon-position="right" %}}Download{{% /button %}}

Download and install *Grass Control v6*. After the mod is installed, som settings needs to be changed.

Double click on the mod in the MO left pane.
Click on the "Text Files" tab to modify GrassControl.config.txt
Find the following settings and edit as follows:

 ```
	UseGrassCache = True
	OnlyLoadFromCache = True
	ExtendGrassDistance = True
	EnsureMaxGrassTypesPerTextureSetting = 15
	OverwriteGrassDistance = 24000 (lower this value for better performance)
	OverwriteGrassFadeRange = 12000 (lower this value for better performance)
	OverwriteMinGrassSize = 60 (Higher values, better performance. Lower value, more grass)
 ```

 Download *Grass Generation MO2 Plugin v1*. Extract the content to *C:/Modding/Tools/Mod Organizer/plugins* (path may need to be corrected to match your paths). Close and restart Mod Organizer.


