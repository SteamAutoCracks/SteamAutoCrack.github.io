# User Manual

<a href="/docs/" class="btn btn-primary">Back</a>

## Main Options

### Path

* Set the Steam clean game file folder (Make sure to choose the root game path, for example in UE4 games you should the folder include `Engine` folder), game executable or steam_api(64).dll.

### Start Crack

* Start the crack process.
* The `Delete Previous steam_settings Folder` is same as  `Goldberg Steam Emulator Configuration`'s.

***

## 1. Generate Goldberg Steam Emulator Game Info

### Steam App ID

* Set the Steam App ID.
* App ID can be found using built-in `App ID Finder` or [SteamDB](https://steamdb.info/).

### Generator API

* Generate game info with different info APIs.
* SteamKit2 Client: Use SteamKit2 Client for generating most of infos and Steam Web API/Xan105 API for game schema. (Best result)
* Steam Web API: Steam Web API/Xan105 API for all game infos. (Faster but less infos)
* Offline: Generate Offline basic info without Internet.

### Use Xan105 API

* Use Xan105 API to replace Steam Web API, but can't generate stats. (Currently not works)

### Steam Web API Key

* Your Steam Web API Key.
* If it's missing without using Xan105 API, game schema (achievements and stats) will not be generated.

### Use Steam Web App List

* Use Steam Web App List for faster game info generating.

### Generate Achievement Images

* Generate game achievement images (icons) for Goldberg Steam emulator. (Now it's much faster)

***

## 2. Generate Goldberg Steam Emulator Configuration

### Language

* Set the language the emulator will report to the game.
* Default language settings will generated from your system language.

### Listen Port

* Set the UDP/TCP port the emulator listens on (You should probably not change this because everyone needs to use the same port or you won't find yourselves on the network).

### Account Name

* Set your name in game.

### Steam ID

* Set your emulator steam id
* If your saves for a game are locked to a specific steam id you need to change this value.

### Disable Networking

* Disable all the networking functionality of the Steam emulator.

### Offline mode

* Enable Steam emulator Offline mode.
* Some games that connect to online servers might only work if the Steam emulator behaves like steam is in offline mode.

### Enable Overlay

* Enable the Steam emulator overlay.
* This is for games that depend on the steam overlay to let people join multiplayer games.
* Use SHIFT-TAB to open the overlay.

### Custom Broadcast IP

* Set custom ips (or domains) which the emulator will send broadcast packets to.

### Open Example Config

* Open Goldberg Emulator Example Folder.

### Open Config Folder

* Open Goldberg Emulator `steam_settings` folder in Temp file.

***

## 3. Unpack SteamStub

* Require Select .exe File or Folder as input path.

### Keep Bind Section

* Keep .bind Section after unpack, required if unpacked executable won't run.

### Use Experimental Features

* Required if unpacked executablewon't run.

### Realign Sections

* Realign executable sections.

### Keep DOS Stub Data

* Keep executable DOS Stub Data.

### Recalculate File Checksum

* Recalculate Executable Checksum.

### SteamAPICheckBypass Mode

* Use [SteamAPICheckBypass](https://github.com/oureveryday/Steam-API-Check-Bypass) to bypass steam_api(64).dll and exe integrity check.
* Disabled: Disable Apply SteamAPICheckBypass.
* SteamAPICheckBypass DLL: DLL Name for DLL hijacking to game executable.
* Enable All Time: Intercept All steam_api(64).dll read request and all game exe read request.
* Enable Only Nth Time: Intercept steam_api(64).dll read request only on Nth time and all game exe read request.
* Enable Only Not Nth Time: Intercept steam_api(64).dll read request only not on Nth time and all game exe read request.
* `Enable Only Nth Time` and `Enable Only Not Nth Time` is useful for custom requirements.
* SteamAPICheckBypass won't intercept `LoadLirary` now.

***

## 4. Apply Goldberg Steam Emulator

* Require Select steam_api(64).dll File or Folder as input path.

### Use Custom Save Location

* Default save path: `C:\Users\<Your windows user name>\AppData\Roaming\Goldberg SteamEmu Saves\<appid>\settings`
* Create a `local_save.txt` beside steam_api(64).dll to change default Goldberg emulator game save path.

### Use Experimental version Goldberg Emulator

* Uses Experimental version Goldberg Emulator.

### Generate Steam Interfaces file

* Automacally Generate steam_interfaces.txt if the original steam_api(64).dll older than may 2016 (Determined with Digital Signature Timestamp).

### Force Generate for each steam_api(64).dll

* Generate steam_interfaces.txt steam_api(64).dll .

***

## 5. Generate Crack Only Files

* Require Select Folder as input path.
* Crack only files will be generated in the `Crack` folder.

### Output Path

* Set the place to put crack only file.

### Create Crack Readme File

* Create Crack_Readme.txt which include infos to apply the crack only file.

### Pack Crack Files with .zip archive

* Pack Crack Files with Crack.zip archive.

***

## 6. Restore Crack

* Require Select Folder as input path.
* Restores Crack Generated with SteamAutoCrack.

***

## AppID Finder

### Fuzzy Search

* If fuzzy search is disabled, will use exact search.

***

## Settings

### Save Config File

* Save Config.json with SteamAutoCrack options.

### Enable Debug Log

* Enable Debug Log Level.

### Output Log to File

* Output all Log to log.log file.
* Error log will always output to error.log regardless of this option is disabled.

### Update/Download

* Update or download latest version Goldberg Steam Emulator if it not exist or a update available.

### Force Update Steam App List

* Update Steam App List now.
* Steam App List will automacally updated daily.
