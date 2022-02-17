# Wrestling Empire Custom Music
A mod for the crazy game Wrestling Empire (PC version) that allows you to add custom character themes by simply putting them in a folder.
**THIS MOD WILL NOT WORK WITH EARLIER OR NEWER VERSIONS THAN SPECIFIED**

# Installation
1. Download the latest release of the mod (found on the right side of this page). I'd recommend downloading the autoinstaller version.  
2. Run the executable called WrestlingEmpireCustomMusicPatcher.exe and a new window will appear.
3. If you downloaded the autoinstaller then no more input is required and you may add all of your favourite songs (read below).
4. If you downloaded the normal version, then find the Assembly-CSharp.dll file in the games folder.
    * This is probably Steam/Steamapps/Wrestling Empire/Wrestling Empire_Data/Managed/Assembly-CSharp.dll
    * A very easy way to get here is to go into Steam, right click Wrestling Empire, hover over manage and click "Browse local files".
      * Then simply go into Wrestling Empire_Data then Managed and it will be the top file if sorted alphabetically.
5. Drag and drop the assembly file onto the console window and press enter. You may have to re-focus the window by clicking on it before pressing enter.

# Updating
1. Go to Steam, right click the game, click Properties, click "Local Files" on the left side, and click "Verify integrity of game files"
2. Follow installation instructions above.

# How to add custom songs
A new folder called Custom Music will be created in the StreamingAssets folder. 
This is in Wrestling Empire/Wrestling Empire_Data/StreamingAssets/
Simply place your .wav, .mp3 and .ogg files in this folder and they will appear in the theme select in the editor the next time you start your game.
Do NOT have any commas in your filenames as it may break the mod, and probably therefor the game. For safety, remove any punctuation from your filenames.

# Uninstalling
Verify the game's files through Steam. You can then delete the Custom Music folder from StreamingAssets if you do not plan on re-installing.
Once you have done this you MUST go into the editor and select each wrestler that used a modded song, making sure the song has been set to None (or anything below 41).
If you don't, the game will try to load the modded song and softlock in a match. 

# Issues
Read through the open issues in the issues tab at the top left of the page. This is where issues are listed. Other than those...
Currently no known real issues. That does not mean there aren't any. Due to the weird way MDickie wrote the game, the game is very fragile and this mod could break anything and everything in an edge scenario.

If you remove a song, you MUST go into the editor and reselect wrestlers that are using a custom song, otherwise the game may break.
Adding a song may swap any modded songs that a character is using. 
  The mod assigns the songs to the numbers alphabetically, so if you add a new song but don't want the order to change, try renaming the song so it appears at the bottom of the folder when sorted alphabetically.
 
As a beneficial upside, this mod (may) also deobfuscate a lot of the code. Feel free to open the assembly dll with a dn decompiler and see what I think is what. 

# Future game updates
Unfortunately, the vast majority of the game is obfuscated. Luckily, however, re-implementing/updating this mod is very simple as most of my code is in a custom class, and only an extremely small portion of the games code is actually touched.

# Can this mod load other custom things like clothing or faces?
No, but making a mod to load that kind of thing is absolutely possible! Hell, it could be really easy but I haven't looked.
This mod basically imports music and adds it to an array. 
I think adding custom textures or models and such should be just as easy, once the correct code is deobfuscated.

# Source code?
Source code for the patcher is not yet available, but it's in C# so you can decompile the executable with something like dnSpy. 
The code is not something I'd like to proudly share, but I might upload it one day.

As for source code of the mod, it's not something I can share without giving away source code of the game. 
If you do own the game though, you can patch a copy of the assembly dll then open it with a dn decompiler, and check out the ModdedMusic class and the SoundManager.LoadTheme() method.
