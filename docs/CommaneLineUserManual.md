# Commane Line User Manual

<a href="/docs/" class="btn btn-primary">Back</a>

* You have to manually compile the CLI version source code.

## Usage

`SteamAutoCrack.CLI [command] [options]`

## Main Commands

Command        | Description
-------------- | --------------
crack \<Path>  | Start crack process.
updateapplist  | Force Update Steam App List.
downloademu    | Download/Update Goldberg Steam emulator.
createconfig   | Create Default Config File.

## Commands

### Crack

Option             | Description
--------------     | --------------
--config <config>  | The process config json file. [Default: config.json in program current running directory]
--appid <appid>    | The game Steam AppID. (Required when Generate Goldberg Steam emulator game info)
--debug            | Enable Debug Log.

### updateapplist

Option             | Description
--------------     | --------------
--debug            | Enable Debug Log.


### downloademu

Option             | Description
--------------     | --------------
--force            | Force (re)download.
--debug            | Enable Debug Log.


### createconfig

Option             | Description
--------------     | --------------
--path <path>      | Changes default config path.
--debug            | Enable Debug Log.
