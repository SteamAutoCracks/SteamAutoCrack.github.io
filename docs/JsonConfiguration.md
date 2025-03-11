---
layout: default
title: SteamAutoCrack Json Configuration Introduction
description: SteamAutoCrack Config.json Configuration Introduction
---

<a href="/docs/" class="btn btn-primary">Back to docs index</a>

# Json Configuration

* GUI version: config.json is created under program folder after enabled `Save Config File`

## Default Config Example

```json
{
  "EMUApplyConfigs": {
    "LocalSave": "steam_settings",
    "UseLocalSave": false,
    "UseGoldbergExperimental": false,
    "GenerateInterfacesFile": false,
    "ForceGenerateInterfacesFiles": false
  },
  "EMUConfigs": {
    "Language": 7,
    "SteamID": "76561197960287930",
    "AccountName": "Goldberg",
    "ListenPort": "47584",
    "CustomIP": "127.0.0.1",
    "UseCustomIP": false,
    "DisableNetworking": false,
    "Offline": false,
    "EnableOverlay": false
  },
  "SteamStubUnpackerConfigs": {
    "KeepBind": true,
    "KeepStub": false,
    "Realign": false,
    "ReCalcChecksum": false,
    "UseExperimentalFeatures": false,
    "SteamAPICheckBypassMode": 0,
    "SteamAPICheckBypassDLL": 0,
    "SteamAPICheckBypassNthTime": [1]
  },
  "EMUGameInfoConfigs": {
    "GameInfoAPI": 0,
    "SteamWebAPIKey": "",
    "GenerateImages": true,
    "UseXan105API": false,
    "UseSteamWebAppList": false
  },
  "GenCrackOnlyConfigs": {
    "OutputPath": "",
    "CreateReadme": false,
    "Pack": false
  },
  "ProcessConfigs": {
    "GenerateEMUGameInfo": true,
    "GenerateEMUConfig": true,
    "Unpack": true,
    "ApplyEMU": true,
    "GenerateCrackOnly": false,
    "Restore": false
  },
  "EnableDebugLog": false,
  "LogToFile": false
}
```

## Description

* Greyed/Code Descriptions is referred to [User Manual](https://github.com/SteamAutoCracks/Steam-auto-crack/wiki/User-Manual)

Key            | Type           | Description
-------------- | -------------- | --------------
EMUApplyConfigs          | Object  | `Apply Goldberg Steam Emulator` config
EMUConfigs               | Object  | `Generate Goldberg Steam Emulator Configuration` Config
SteamStubUnpackerConfigs | Object  | `Unpack SteamStub` config
EMUGameInfoConfigs       | Object  | `Generate Goldberg Steam Emulator Game Info` config
GenCrackOnlyConfigs      | Object  | `Generate Crack Only Files`
ProcessConfigs           | Object  | Select processes to process
EnableDebugLog           | Boolean | Output debug log as log.log (GUI Only)
LogToFile                | Boolean | Output log to file (GUI Only)

### EMUApplyConfigs

Key            | Type           | Description
-------------- | -------------- | --------------
LocalSave          | String  | `Use Custom Save Location` Path
UseLocalSave               | Boolean  | `Use Custom Save Location`
UseGoldbergExperimental | Boolean  | `Use Experimental version Goldberg Emulator`
GenerateInterfacesFile       | Boolean  | `Generate Steam Interfaces file`
ForceGenerateInterfacesFiles      | Boolean  | `Force Generate for each steam_api(64).dll`

### EMUConfigs

Key            | Type           | Description
-------------- | -------------- | --------------
Language          | Number(Enum)| `Language` 0-28 in following order: `"arabic, bulgarian, schinese, tchinese, czech, danish, dutch, english, finnish, french, german, greek, hungarian, italian, japanese, koreana, norwegian, polish, portuguese, brazilian, romanian, russian, spanish, latam, swedish, thai, turkish, ukrainian, vietnamese"`
SteamID              | String   | `Steam ID`
AccountName | String   | `Account Name`
ListenPort       | String   | `Listen Port`
CustomIP     | String   | `Custom Broadcast IP`
UseCustomIP| Boolean| Enable `Custom Broadcast IP`
DisableNetworking|Boolean| `Disable Networking`
Offline|Boolean| `Offline mode`
EnableOverlay|Boolean| `Enable Overlay`

### SteamStubUnpackerConfigs

Key            | Type           | Description
-------------- | -------------- | --------------
KeepBind|Boolean| `Keep Bind Section`
KeepStub|Boolean| `Keep DOS Stub Data`
Realign|Boolean| `Realign Sections`
ReCalcChecksum|Boolean| `Recalculate File Checksum`
UseExperimentalFeatures|Boolean| `Use Experimental Features`
SteamAPICheckBypassMode|Number(Enum)| `SteamAPICheckBypass Mode` 0-3 in following order: `"Disabled,Enable All Time,Enable Only Nth Time,Enable Only Not Nth Time"`
SteamAPICheckBypassDLL|Number(Enum)| `SteamAPICheckBypass DLL` 0-2 in following order: `"winmm.dll,version.dll,winhttp.dll"`
SteamAPICheckBypassNthTime|Int64| The List of Nth Time when use `Enable Only Nth Time` and `Enable Only Not Nth Time` mode.


### EMUGameInfoConfigs

Key            | Type           | Description
-------------- | -------------- | --------------
GameInfoAPI|Number(Enum)| `Generator API` 0-2 in following order: `"SteamKit2 Client,Steam Web API,Offline"`
SteamWebAPIKey|String| `Steam Web API Key`
GenerateImages|Boolean| `Generate Achievement Images`
UseXan105API|Boolean| `Use Xan105 API`
UseSteamWebAppList|Boolean| `Use Steam Web App List`

### GenCrackOnlyConfigs

Key            | Type           | Description
-------------- | -------------- | --------------
OutputPath|String| `Output Path`
CreateReadme|Boolean| `Create Crack Readme File`
Pack|Boolean| `Pack Crack Files with .zip archive`

### ProcessConfigs

Key            | Type           | Description
-------------- | -------------- | --------------
GenerateEMUGameInfo|Boolean| Enable `Generate Goldberg Steam Emulator Game Info`
GenerateEMUConfig|Boolean| Enable `Generate Goldberg Steam Emulator Configuration`
Unpack|Boolean| Enable `Unpack SteamStub`
ApplyEMU|Boolean| Enable `Apply Goldberg Steam Emulator`
GenerateCrackOnly|Boolean| Enable `Generate Crack Only Files`
Restore|Boolean| Enable `Restore Crack`