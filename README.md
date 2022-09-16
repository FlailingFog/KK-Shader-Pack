# KK Blender Porter Pack
Plugin pack for exporting and setting up Koikatsu characters in Blender.  

The ```KKBP exporter for Koikatsu``` is used to export the character's mesh, armature and color data. The exported data is then processed by the ```KKBP plugin for Blender```. Once characters are setup in Blender, they can be saved as FBX files for use in other programs. 

The changelog for the pack [can be found here.](https://github.com/FlailingFog/KK-Blender-Shader-Pack/blob/master/Changelog.md)
The pack [also has a barebones wiki here.](https://github.com/FlailingFog/KK-Blender-Shader-Pack/wiki)

# Download
Stable versions of KKBP are [on the release page](https://github.com/FlailingFog/KK-Blender-Porter-Pack/releases).  
The latest version of KKBP can be downloaded by using the green CODE button on the top right of the page and choosing "Download ZIP"

# Usage Instructions for V6
### Exporting from Koikatsu and importing to Blender
<details><summary>Click to expand</summary> 

#### Prerequisites:
* Install [HF Patch v3.16 or later](https://github.com/ManlyMarco/KK-HF_Patch) for Koikatsu or [HF Patch v1.7 or later](https://github.com/ManlyMarco/KKS-HF_Patch) for Koikatsu Sunshine
* Install either [CATS](https://github.com/GiveMeAllYourCats/cats-blender-plugin) or [mmd_tools](https://github.com/UuuNyaa/blender_mmd_tools) for Blender

1. Install KKBP for Koikatsu by copying the KKBP_Exporter.DLL into the plugins folder: C:/Koikatsu install directory/BepInEx/plugins/  
    a. Use the net3.5 exporter for Koikatsu and Koikatsu Party  
    b. Use the net4.6 exporter for Koikatsu Sunshine
1. Start the game, go to the character creator and load your character
1. Click the "Export Model for KKBP" button on the top of the screen. This may take a few minutes depending on your hardware. A folder will popup when the export is finished  
![ ](https://github.com/FlailingFog/KK-Blender-Porter-Pack/blob/assets/readme/exportpanel.PNG)
1. Copy the entire folder generated by the plugin to your desktop. This folder is located in C:/Koikatsu install directory/Export_PMX. The format of this folder is ######_CharacterName.
1. Install KKBP for Blender through the addon menu
1. Click the Import Model button in the KKBP panel and choose the .pmx file from the export folder. This may take a few minutes depending on your hardware.  
![ ](https://github.com/FlailingFog/KK-Blender-Porter-Pack/blob/assets/readme/panelimport.PNG)
</details>

### Exporting from Blender

<details><summary>Click to expand</summary> 

1. Save a backup file of your finished model
1. Choose which export type you want in the KKBP panel. There's currently a targeted export type for Unity (VRM), and a generic fbx type for everything else
1. Click the "Prep for target application" button
1. Click the "Bake material templates" button and choose the folder you want to store all of your baked images to (warning: there's going to be a lot, so an empty folder is recommended)
1. Create an altas for the body, clothes and hair objects using the [material combiner](https://github.com/Grim-es/material-combiner-addon) addon
1. Hit the undo button to return to the state before you created the atlas. Change the menu under the "Apply baked templates" button to "Dark" and click the button to load in the dark textures. Use material combiner again to generate the dark version of the material atlas 
1. Click the export FBX button to invoke the built-in fbx export dialog
</details>

# Similar Projects

* [Koikatsu Pmx Exporter (Reverse Engineered & updated)](https://github.com/Snittern/KoikatsuPmxExporterReverseEngineered)
* [KKPMX](https://github.com/CazzoPMX/KKPMX)
* [Grey's mesh exporter for Koikatsu](https://www.google.com/search?q=koikatsu+discord)
