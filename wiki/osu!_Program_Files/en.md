# osu! program files

![The file structure of osu!'s installation folder](img/osu!-program-files.png "The file structure of osu!'s installation folder")

### Installation Paths ###
<!--TODO: Find out where macOS osu! is stored-->
osu! is installed by default in the following locations, by default:
| Windows 	| C:\Users\<username>\AppData\Local\osu! 	|
|---------	|----------------------------------------	|
| Mac     	|                                        	|

## Folders

### Chat

This folder only appears if you have "Automatically log private messages" enabled in Options, or you run the "/savelog" command in the [Chat Console](/wiki/Chat_Console).

The file name structure is `{Tab_name}-{YYYYMMDD}-{HHMMSS}`, and can be opened in any text editor (e.g. Notepad)

**Example**: #multiplayer-20121115-040845 (/savelog at #multiplayer tab in 15th November 2012 at 04hrs, 08mins, and 45secs).

### Downloads

This folder holds the beatmaps being downloaded by osu!direct (requires [osu!supporter](/wiki/osu!supporter)). They get transferred to the Songs folder upon completion.

### Exports

This folder appears if you use the [Skin Selector's "Export as .osk"](/wiki/Options) or [Beatmap Editor's "Export Package"](/wiki/Beatmap_Editor/Menu). It will hold the beatmaps and skins you have exported from osu!.

If you want to know how to do this, see [osu! File Formats](/wiki/osu!_File_Formats).

### Localisations

This folder holds your replay files. A replay file does not work when the beatmaps linked to it is missing. The replay also contains the results data, and reanimates your cursor movement while replaying. To create a replay, press F2 at the results screen, or click on the 'Save replay to Replays folder' (in Solo only). This, however, does not save multi-play elements. The file sizes in here are usually ranging from 100KB ~ 1KB. [For players who are interested to upload their replay to YouTube, see this thread](https://osu.ppy.sh/community/forums/topics/1104243).

The format is `{Local player name} - {Artist} - {Title} {[Difficulty]}{(YYYY-MM-DD)} {Game Mode}`

**Example:** dummytest1 - Loituma - Ievan Polkka \[SPINNER-MADNESS\]  (2013-08-12) OsuMania

### Screenshots

**This folder holds screenshots you have created in osu!**. The saved screenshot's file extension (.jpg/.png) is based on what you set on the Options menu.

To create a screenshot, press the screenshot key (F12 by default).

The file name structure is `screenshot###`, where "###" is the screenshot number count.

### Skins

This folder holds **user-created skins, which can be used to customise the in-game interface.** You can download skins from the [Skinning subforum](https://osu.ppy.sh/community/forums/15). You can instal skins by double-clicking on the skin from a file manager. If the downloaded skin is in folder form, you will have to place the folder here yourself. If it is in a ZIP or RAR format, you must extract it first. You can change your skins at [Options menu under Skins tab (Skin Selector)](/wiki/Options). Please bear in mind that the selected skin is only visible to you.

For further reference, please refer to the [Skinning](/wiki/Skinning) page. Also, "osu! by peppy" is the only skin without its folder and cannot be deleted.

### Songs

**This folder holds all your osu! beatmaps**. Usually contains .osu (difficulties), .mp3/.ogg (music files), .jpg/.png/.gif (background images), .osb (storyboard files) and .mp4/.flv (video files). May also contains .wav/.ogg (hitsound files) and folders (storyboard spites and/or skin).

The file name structure is `{Beatmap number} {Artist} - {Song Title}`.
**Example:** [57950 SOUND HOLIC - Drive My Life](https://osu.ppy.sh/beatmapsets/57950)

Please note that some very old beatmaps (for example, [Kenji Ninuma - DISCO PRINCE](https://osu.ppy.sh/beatmapsets/1) or [Dudelstudios - Angry Video Game Nerd Theme [MATURE CONTENT]](https://osu.ppy.sh/beatmapsets/66)), as well as unsubmitted beatmaps, do not follow the format.

## Hidden Folders

*Caution: Be careful with these files, you might break osu! if you are not careful.*

### Data

osu!data files. They should not be tampered with.

## Files

### Database Files (.db)

The .db files are beatmaps' data which only osu! can utilise.

**osu! database**

- collection.db (Your "Collections" in-game. You can post it to forum for others to check out your "Collections". Actual beatmaps not provided.)
- osu!.db (osu! beatmaps' cache.)
- presence.db (Cache of osu!players logged in the Chat_Console)
- scores.db (Stores historical local scores)

### .cfg (Configuration files)

Configuration files or config files configure the initial settings for osu! to work. The files can be opened by Notepad.

- `osu!.cfg`: Stores security information about the osu! application files and current release stream. This should never be modified manually.
- `osu!.<username>.cfg`: Stores [Options](/wiki/Options) data and other game settings. See [User Configuration File](/wiki/osu!_Program_Files/User_Configuration_File).

<!--TODO: Find out what osu!'s executable is in other platforms.
### .exe (Application)

The main component. Click on it to start-up. The .exe files are safe to open assuming you used the osu!installer to install osu!.

osu!.exe (Start-up osu!)-->

#### .dll (application extension)

These .dll files are components of osu!, and osu!'s dependencies.

**Dependencies**

- avcodec-51.dll
- avformat-52.dll
- avutil-49.dll
- bass.dll
- bass_fx.dll
- d3dcompiler_47.dll
- libEGL.dll
- libGLESv2.dll
- Microsoft.Ink.dll
- OpenTK.dll
- pthreadGC2.dll

**osu! components**

- osu!gameplay.dll
- osu!seasonal.dll
- osu!ui.dll
- osu.dll
