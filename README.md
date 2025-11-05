# Split/Second Archipelago Manual Implementation
An Archipelago Manual implementation for the PC game Split/Second. Intended to be played through using a blank save in Season mode.

## Randomizer Details
### Goal
The manual has 2 goals to choose from:
1. Complete all 12 Episodes and come in 3rd or higher in the the Elite Race of the final Episode "Out With A Bang".
2. Complete the "Perfection" Decal, finishing in 1st in all Events.

### Progression
There are 2 methods of Episode progression, available through YAML options:
1. Normal: Episodes are locked behind seperate items, and you cannot enter Episodes that you have not unlocked yet.
2. Progressive: Unlocks are replaced by generic "Progressive Episode" items, to prevent getting stuck as much. Follows the philosophy of always picking the leftmost episode during selection.

### Items
All cars are locked as Items (with some tweaks available through YAML options). Car variants are available as Filler Items.

All Episodes are locked as Items, except the first (Rigged to Blow).

Optionally, the ability to use Power Plays can be locked as Items as well.

### Locations
Every Event has 2 Locations, one for completion and one for getting a Win, though the definition of a 'Win' is up to the player.

Credit thresholds for unlocking cars are additional Locations.

Wreck thresholds for unlocking the Bonus Event in each Episode are also Locations.

Optionally, you can set the various Decals (effectively achievements) as Locations. These exclude online-based achievements as well as 'Have We Met Before?' for owning Pure.

### Traps
2 Trap categories are available.

Random Car Trap: Forces the player to use a random unlocked car for the next Event, until one is completed. Randomization method is up to the player.

Forced Power Play Trap: Forces the next Power Play that appears to be triggered. The method used to ensure the Power Play triggers is up to the player. Examples include repeatedly tapping the Power Play keys or turning on an autoclicker.

## Additional Details & Caveats
The base game has a bug in Episode 6 where the save file becomes corrupted until an Event in Episode 7 is completed. You can wait until an Episode after 6 is available, or create a backup save.

Since Elite Races force you to choose the next Episode upon completion, they're only in logic once one of the next Episodes are available.

An additional "splitsecond.params" file is available, which unlocks all cars. This helps if using Non-Progressive Car unlocks.

## Installation Instructions
1. Downlaod the provided APWorld.
2. Double-click to install the world into Archipelago.
3. Open Archipelago and click "Generate Template Options" to create the YAML in the "Archipelago/Players/Templates" folder. It should be labelled "Manual_SplitSecond_UnProx.yaml".
4. Edit the YAML to your liking.
5. (Optional) If using Non-Progressive Car unlocks, additionally download the "splitsecond.params" file and place it in the same folder as your "SplitSecond.exe" game.
