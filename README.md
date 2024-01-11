# osu-replay-analysis-tool
ORAT (osu! replay analysis tool) is a program the detects if a player is using cheats using .osr (osu! Replay) files, coded by someone with extensive knowledge of how osu! cheats work.

## What cheats/hacks does it detect
### Timewarp
It uses Replay Frames to see if the rate of frames is invalid, if so the player most likely used Timewarp.

### Relax
Determines if the player used Relax in the replay using multiple methods.

Method 1: This detects Relax if the UR is less than or equal to a set value (for example 30).

Method 2: This detects Relax if the holding time if suspiciously close to the actual hold time of the hit objects.

Method 3: This detects Relax if the player singletaps a set BPM or above.

### Aim Assist/Other related aim cheats
Determines if the player is using Aim cheats using multiple methods.

Method 1: Determines if the player is using Aim cheats by checking if the mouse cursor is exactly/on a certain position on a hit object.

Method 2: Determines if the player is using Aim cheats by detecting suspicious snaps.

Method 3: Determines if the player is using Aim cheats by detecting cursor teleports, can false flag TD plays though.

Method 4: Detects if a player aims a certain way that is similar to Aimbot/Aim Assist, if so they are most likely using Aim cheats.

### Replay Copier
Detects if the player's cursor movement/tapping is VERY similar to an already existing replay.

### Replay Editor/Difficulty Changer
Calculates 300s, 100s, 50s, and other things using replay frames and compares them to the replay data to see if a player is using replay editor and/or difficulty modification cheats.
