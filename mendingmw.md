# INDEX

- [Mending Morrowind](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#mending-morrowind)
  - [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#morrowind-code-patch)
  - [High resolution textures](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#high-resolution-textures)
  - [Bug fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#bug-fixes)
  - [Optimization](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#optimization)
  - [Expansion delay](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#expansion-delay)
  - [Official plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#official-plugins)
  - [.INI edits](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#ini-edits)
  - [Load order](https://github.com/Sigourn/morrowind-improved/blob/master/mendingmw.md#load-order)
- [Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

# MENDING MORROWIND

## Morrowind Code Patch

The Morrowind Code Patch patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays with vanilla Morrowind, as opposed to OpenMW.

Unlike mods, the Morrowind Code Patch requires specific install instructions, and can't be installed through Mod Organizer 2.

1. First, download the **Morrowind Code Patch** main file from [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files).
2. Extract the contents of the file to your Morrowind root directory, so that Morrowind Code Patch.exe and the mcpatch folder are in the same folder as Morrowind.exe.
3. Now download the **MCP beta** update file from [**Morrowind Code Patch Update**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files).
4. Extract the contents of the file to your Morrowind root directory, and overwrite when prompted. This will update the Morrowind Code Patch to version 2.5b4.
5. Right click on Morrowind Code Patch.exe and select **Run as Administrator**.
6. The amount of options available can be overwhelming. My recommendation is to install or skip patches as per [**this handy Google Sheets document**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing).

Once you finish installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your Morrowind folder, and you will be done.

## High resolution textures

This mod list does not condone the use of using texture replacers for the sake of it. However, that does not mean the purist Mororwind player is out of good alternatives for the vanilla textures.

- [**Morrowind Uncompressed Vanilla Textures**](https://www.nexusmods.com/morrowind/mods/45551) by Bethesda Softworks: replaces most vanilla textures with unused textures that have less compression artifacts found in the game's Data Files folder.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros: replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and click **OK**.
  - Now install a second instance of this mod. This time, tick **01 Atlas Textures** and click **OK**.
  - MO2 will tell you the mod already exists. Click **Rename**. I suggest modifying it to read **Intelligent Textures v2.1 - Atlas Textures**. Click **OK**.
  - Also install the **Wood Fix** update file.
  - Also install [**this hotfix**](https://www.mediafire.com/file/impju2r934eqkkt/Intelligent_Textures_Ashlander_Hotfix_v2.zip/file), which will fix a bug with one of the ashlander hairstyles.

## Bug fixes

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11: unofficial patch that aims to make the game completely bug-free (within the abilities of TESCS). In addition to being under active development, it diverges from later versions of the community patches in that it aims to only fix bugs (avoiding unnecessary balance and gameplay changes), takes a more conservative approach about what it considers a bug, and implementing bug fixes in coordination with Tamriel Rebuilt and the Project Tamriel projects.
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich: fixes UV mapping on rocks and stones.
- [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634) by NullCascade: forces the game to instantly close on exit.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich: fixes issues regarding light sources in the game.
  - Hide/deactivate **Glowing Flames - TrueLightsAndDarkness Tweaks.esp**.
- [**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947) by Petethegoat: normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement. 
- [**No More Stage Diving - Desele's Dancing Girls**](https://www.nexusmods.com/morrowind/mods/47738) by Pherim: keeps the girls in Desele's House of Earthly Delights from dancing off the stage by making them not greet the player as he approaches them. 
  - Only install the **No More Stage Diving** main file.
  - Hide/deactive **NoMoreStageDiving_TalkativeGirls.esp**.
- [**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269) by Merzasphor: makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.
- [**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029) by Merzasphor: fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

## Optimization

- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7: greatly improves performance and fixes some mesh errors. MO2 will install the mod as a BAIN package. Tick **all options** and click **OK**.
  - Hide/delete **meshes\f\furn_web00.nif** and **meshes\f\furn_web10.nif**. These meshes are buggy and cause visual problems when seen from a distance.
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team: optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and click **OK**.
  - Hide/delete **meshes\x\ex_imp_plat_01.nif**. This mesh is buggy and can cause problems when traveling from Raven Rock to Fort Frostmoth using the boat.

## Expansion delay

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11: modifies how the Tribunal and Bloodmoon expansions are implemented into the game.

## Official plugins

Bethesda released a number of official plugins for Morrowind, which already come with the Morrowind: Game of the Year Edition available from GOG. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

My personal stance, and the one which this guide follows, is: don't bother with them. I recommend you remove the following plugins from your game:

- adamantiumarmor.esp
- AreaEffectArrows.esp
- bcsounds.esp
- EBQ_Artifact.esp
- entertainers.esp
- LeFemmArmor.esp
- master_index.esp
- Siege at Firemoth.esp

## .INI edits

The Morrowind Code Patch **Rain/snow collision** patch requires a few .ini edits to work properly.

- Launch Mod Organizer 2.
- Click on the **Tools** icon, which resembles a jigsaw puzzle, and select **INI Editor**.
- On the morrowind.ini that just opened, adjust the following values. Use CTRL+F to input the bolded names and find them easily.
  - **[Weather Rain]**
  - Rain Diameter=600 -> Change this to **Rain Diameter=1200**
  - Max Raindrops=450 -> Change this to **Max Raindrops=1500**
  - **[Weather Thunderstorm]**
  - Rain Diameter=600 -> Change this to **Rain Diameter=1200**
  - Max Raindrops=650 -> Change this to **Max Raindrops=3000**
  - **[Weather Snow]**
  - Snow Diameter=800 -> Change this to **Snow Diameter=1600**
  - Max Snowflakes=750 -> Change this to **Max Snowflakes=1500**
- Click Save to finish editing the Morrowind.ini.

## Load order

[**Refer to this section**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#mod-order-and-load-order) to know what the appropiate mod order and plugin load order is for these mods.