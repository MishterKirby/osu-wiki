# osu! program files

![The file structure of osu!'s installation folder, on Windows and macOS](img/file_structure.png "The file structure of osu!'s installation folder, on Windows and macOS")
The **osu! program files** are a set of files that run osu! and keep track of different activities as user's play.

### Installation Paths ###

osu! is installed in the following locations, by default:
| Windows | macOS |
| :-- | :-- |
| `C:\Users\<Username>\AppData\Local\osu!` | `/Applications/osu!.app/Contents/drive_c/osu`! |

## Folders

### Chat

The Chat folder only appears if the player has "Automatically log private messages" enabled in Options, or the player runs the "/savelog" command in the [Chat Console](/wiki/Chat_Console).

The name structure of the files is `{Tab_name}-{YYYYMMDD}-{HHMMSS}`, and can be opened in any text editor. An example of this is shown below:

**Example**: #multiplayer-20121115-040845 (/savelog at #multiplayer tab in 15th November 2012 at 04hrs, 08mins, and 45secs).

### Downloads

The Downloads folder holds the beatmaps being downloaded by osu!direct (requires [osu!supporter](/wiki/osu!supporter)). They get transferred to the Songs folder upon completion.

### Exports

The Exports folder appears if the player uses the [Skin Selector's "Export as .osk"](/wiki/Options) or [Beatmap Editor's "Export Package"](/wiki/Beatmap_Editor/Menu). It will hold the beatmaps and skins the player has exported from osu!.

Players that want to know how to do this can see [osu! File Formats](/wiki/osu!_File_Formats).

### Localisations

The Localizations folder appears when the player has switched their language in the options. It will hold the translated text files which can be used each to replace the English text based on the user's selected localisation.

### Replays
The Replays folder holds the player's replay files. A replay file does not work when the beatmaps linked to it is missing. The replay also contains the results data, and reanimates the player's cursor movement while replaying. To create a replay, press F2 at the results screen, or click on the 'Save replay to Replays folder' (in Solo only). [For players who are interested to upload their replay to the YouTube, see this thread](https://osu.ppy.sh/community/forums/topics/1104243).

The file name structure is `{Local player name} - {Artist} - {Title} {[Difficulty]}{(YYYY-MM-DD)} {Game Mode}`

**Example:** dummytest1 - Loituma - Ievan Polkka \[SPINNER-MADNESS\]  (2013-08-12) OsuMania

### Screenshots

**The Screenshots folder holds screenshots the player has created in osu!**. The saved screenshot's file extension (.jpg/.png) is based on what the player set on the Options menu.

*Note: To create a screenshot, press the screenshot key (F12 by default).*

The file name structure is `screenshot###`, where "###" is the screenshot number count.

### Skins

The Skins folder holds **user-created skins, which can be used to customise the in-game interface.** Players can download skins from the [Skinning subforum](https://osu.ppy.sh/community/forums/15). Players can install skins by double-clicking on the skin from a file manager. 

*For further reference, please refer to the [Skinning](/wiki/Skinning) page.*` "osu! by peppy" is the only skin without its folder and cannot be deleted.

### Songs

**The Songs folder holds the player's osu! beatmaps**. Usually contains `.osu` (difficulties), `.mp3`/`.ogg` (music files), `.jpg`/`.png`/`.gif` (background images), `.osb` (storyboard files) and `.mp4`/`.flv` (video files). May also contain `.wav`/`.ogg` (hitsound files) and folders (storyboard spites and/or skin folders).

The file name structure is `{Beatmap number} {Artist} - {Song Title}`.
**Example:** [57950 SOUND HOLIC - Drive My Life](https://osu.ppy.sh/beatmapsets/57950)

Please note that some very old beatmaps (for example, [Kenji Ninuma - DISCO PRINCE](https://osu.ppy.sh/beatmapsets/1) or [Dudelstudios - Angry Video Game Nerd Theme [MATURE CONTENT]](https://osu.ppy.sh/beatmapsets/66)), as well as unsubmitted beatmaps, do not follow the format.

## Hidden folders
These folders are hidden because any modifications to them could prevent osu! from starting correctly, or at all.
### Data

osu! data files. Contains some of osu!'s cache, like beatmap background cache and avatar caches. They should not be deleted, because they may be in use by osu!.

### Files

*Caution: Be careful with these files, you might break osu! if you are not careful.*

## Database files (.db)

The database files are daabases that osu! requires to function propertly. The files contain vital information that osu! requires, such as saved scores, and the list of beatmaps saved on the player's device.

- `collections.db`: Stores the player's "Collections" in-game. The player can post them to the forums for others to see. Actual beatmaps are not provided with the collection file.
- `osu!.db`: Stores osu!'s database of beatmaps.
- `presence.db`: Stores a cache of osu!players logged in the Chat Console.
- `scores.db`: Stores the local leaderboards.
## .cfg (Configuration files)

Configuration files or config files configure the initial settings for osu! to work. The files can be opened with a text editor.

- `osu!.cfg`: Stores security information about the osu! application files and current release stream. This should never be modified manually.
- `osu!.<username>.cfg`: Stores [Options](/wiki/Options) data and other game settings. See [User Configuration File](/wiki/osu!_Program_Files/User_Configuration_File).


### .exe (Application)

The main component. Click on it to start-up (only applies to Windows.) The .exe files are safe to open assuming the player used the osu!installer to install osu!.

osu!.exe (Start-up osu!)

#### .dll (application extension)

These .dll files are osu!'s components and dependencies.

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
- osu.dll
- osu!auth.dll 
- osu!gameplay.dll
- osu!seasonal.dll
- osu!ui.dll
