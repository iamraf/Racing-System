# `race.inc`

Racing System for GTA San Andreas Multiplayer (SA-MP)

This system was originally created for my server. With few changes, script is now **plug-n-play**.

I have made few notes in the script (search `NOTICE`) in case you want to check them and act accordingly.

Tested on bare.pwn.

## Features

- Supports as many races as you like
- Realistic positioning
- Records

## Commands
- `/race` - Add player in race
- `/startrace` - Select and start any race
- `/endrace` - End race before it's finishing time
- `/records` - List all races records
- `/resetrecord` - Reset a specific record
  
## Requirements

- [sscanf](https://github.com/maddinat0r/sscanf/releases)
- [foreach](https://github.com/karimcambridge/SAMP-foreach)
- [zcmd](https://pastebin.com/SbJc7iXa)
  
## Installation:

- Download `race.inc` and `Race` folder
- Move `race.inc` to `./pawno/include/` 
- Move `Race` folder into `./scriptfiles/`
- Add `#include <race>` in your script
- Profit
	
 ## How to add Race:
 
- Go to `./scriptfiles/Race/` folder
- Create new `.txt` file
- In the first line add your Race properties separated with `|` 
	- RaceName
	- VehicleID
	- MaxCheckpoints
	- Interior
	- VehiclesDistance
	- Record
	- RecordPlaced
	- RecordHolder
	- SpawnPositionX
	- SpawnPositionY
	- SpawnPositionZ
	- SpawnPositionA
- Add your Checkpoints `X|Y|Z` separated with `|`
- Name the file with the total of races starting from `0`
- Change `MAX_RACES` to your total races
