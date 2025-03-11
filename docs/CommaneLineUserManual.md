---
layout: default
title: SteamAutoCrack Command Line User Manual
description: Command Line User Manual
---

<a href="/docs/" class="btn btn-primary">Back to docs index</a>

# Command Line User Manual  

* You have to manually compile the CLI version source code.

## Usage

`SteamAutoCrack.CLI [command] [options]`

## Main Commands

Command        | Description
-------------- | --------------
crack \<Path>  | Start the crack process.
updateapplist  | Force update of the Steam App List.
downloademu    | Download/Update the Goldberg Steam emulator.
createconfig   | Create a default config file.

## Commands

### Crack

Option         | Description  
-------------- | --------------
--config <config>  | The process configuration JSON file. [Default: `config.json` in the program's current running directory]  
--appid <appid>    | The game's Steam AppID. (Required when generating Goldberg Steam emulator game info)  
--debug            | Enable debug logging.  

### updateapplist

Option  | Description
------- | --------------
--debug | Enable debug logging.

### downloademu

Option   | Description
-------- | --------------
--force  | Force (re)download.
--debug  | Enable debug logging.

### createconfig

Option        | Description
------------- | ------------------------------
--path <path> | Change the default config path.
--debug       | Enable debug logging.