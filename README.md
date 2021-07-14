# Wrestling Empire Custom Music
A mod for the PC crazy game Wrestling Empire that allows you to add custom character themes by simply putting them in a folder.
Currently for version v1.2

# Installation
1. Run the executable called WrestlingEmpireCustomMusicPatcher.exe and a new window will appear.
1. Find the Assembly-CSharp.dll file in the games folder. 
    * This is probably Steam/Steamapps/Wrestling Empire/Wrestling Empire_Data/Managed/Assembly-CSharp.dll
    * A very easy way to get here is to go into Steam, right click Wrestling Empire, hover over manage and click "Browse local files".
       * Then simply go into Wrestling Empire_Data then Managed and it will be the top file if sorted alphabetically.
1. Drag and drop the assembly file onto the console window and press enter. You may have to re-focus the window by clicking on it before pressing enter.

# How to add custom songs
A new folder called Custom Music will be created in the StreamingAssets folder. 
This is in Wrestling Empire/Wrestling Empire_Data/StreamingAssets/
Simply place your .wav, .mp3 and .ogg files in this folder and they will appear the next time you start your game.

# Issues
Currently no known real issues. That does not mean there aren't any. Due to the weird way MDickie wrote the game, the game is very fragile and this mod could break anything and everything in an edge scenario.

If you remove a song, any character using a modded song will either be using the next song up, or will have their song set to none.
  Adding a song may also swap any modded songs that a character is using. 
  In either of these cases, simply choose the song again.
  
A file will get created called IndexListFile. This file is a relic that doesn't really matter, but I haven't removed yet.

As a beneficial upside, this mod also deobfuscates a lot of the code. Feel free to open the assembly dll with a dn decompiler and see what I think is what. 
  Some of it is purely wrong, but a lot of it is right (as far as I can tell).

# Future updates
Unfortunately, the vast majority of the game is deobfuscated. Luckily, however, re-implementing/updating this mod should pretty simple as most of my code is in a custom class, and only a small portion of the games code is actually touched.

# Can this mod load other custom things like clothing or faces?
No, but making a mod to load that kind of thing is absolutely possible! Hell, it could be really easy but I haven't looked.
This mod basically imports music and adds it to an array. 
I think adding custom textures or models and such should be just as easy, once the correct code is deobfuscated.
