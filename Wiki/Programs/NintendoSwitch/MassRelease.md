# Mass Release

## Program Description

MassRelease will release entire boxes of Pokémon. The main use case is getting rid of breedjects and non-shiny fossils.

### Setup of Settings

1. Text Speed: Fast
2. Casual mode: Off

### Box Setup

1. Place entire boxes filled with Pokémon to be released consecutively.
2. All boxes marked for deletion must be full.
   1. This program does not tolerate partial boxes.

### Instructions

1. You must in the box system.
2. The cursor must be over the 1st Pokémon in the box. (top-left corner)
3. The cursor must be red. (not blue or green)
4. Start the program in the [Change Grip/Order Menu](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Appendix:-ChangeGripOrderMenu).

   > Once started, this program will release the specified number of boxes consecutively starting from the current box.

### Required Parameters:
- `BOXES_TO_RELEASE`: You must specify the number of boxes to release.

### Safety Recommendations:
See [Maximizing Switch Stability](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Appendix:-MaximizingSwitchStability).

***

### Options

This program does not use the global setting to bypassing the system update window. It has its own setting for that. (See below.)

### # of Boxes to Release:
```
const uint8_t BOXES_TO_RELEASE  =   2;
```
This is the number of boxes to release.

### Dodge the System Update Window:
```
const bool DODGE_SYSTEM_UPDATE_WINDOW   =   false;
```
When set to true, the program will dodge the system update window. Do not set this option if the system update window is not present. Unlike other programs, MassRelease will not be able to tolerate the extra button presses if they land in the box system.
