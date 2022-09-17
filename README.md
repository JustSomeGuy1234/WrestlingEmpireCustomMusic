# Wrestling Empire Custom Music
A mod for the crazy game Wrestling Empire (PC version) that allows you to add custom character themes by simply putting them in a folder.
**THIS MOD WILL NOT WORK WITH EARLIER OR NEWER VERSIONS THAN SPECIFIED**

# Installation
Refer to the tutorial text file in this repository or https://youtu.be/LY98dSBa2x4
I am no longer releasing patches so follow the tutorial(s).

# Updating
To reinstall after an update, follow the above tutorial(s).

# How to add custom songs
A new folder called Custom Music must be created in the StreamingAssets folder. 
This must be in Wrestling Empire/Wrestling Empire_Data/StreamingAssets/
Simply place your .wav, .mp3 and .ogg files in this folder and they will appear in the theme select in the editor the next time you start your game.
For reliability, remove any punctuation from your filenames.

# Uninstalling
Verify the game's files through Steam. You can then delete the Custom Music folder from StreamingAssets if you do not plan on re-installing.
Once you have done this you MUST go into the editor and select each wrestler that used a modded song, making sure the song has been set to None (or anything below 69).
If you don't, the game will try to load the modded song and softlock in a match. 

# Issues
Read through the open issues in the issues tab at the top left of the page. This is where issues are listed.

If you remove a song, you MUST go into the editor and reselect wrestlers that are using a custom song, otherwise the game may break.
Adding a song may swap any modded songs that a character is using. 
  The mod assigns the songs to the numbers alphabetically, so if you add a new song but don't want the order to change, try renaming the song so it appears at the bottom of the folder when sorted alphabetically.
 

# Can this mod load other custom things like clothing or faces?
No, but making a mod to load that kind of thing is absolutely possible! Hell, it could be really easy but I haven't looked.
This mod basically imports music and adds it to an array. 
I think adding custom textures or models and such should be just as easy, once the correct code is deobfuscated.

# Source code?
Mod source code can be found in the tutorial text file.
