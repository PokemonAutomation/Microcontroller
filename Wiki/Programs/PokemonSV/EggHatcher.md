# Egg Hatcher

**Related Programs:**
- **Microcontroller:** [Egg Hatcher](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSV/EggHatcher.md) (this program)
- **Microcontroller:** [Egg Combined](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSV/EggCombined.md)
- **Microcontroller:** [Egg Fetcher](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSV/EggFetcher.md)
- **Computer Control:** [Egg Fetcher](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/EggFetcher.md)
- **Computer Control:** [Egg Hatcher](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/EggHatcher.md)
- **Computer Control:** [Egg Autonmous](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/EggAutonomous.md)

The microcontroller and computer-control versions of this program are conceptually similar, with the microcontroller version being less error tolerant without capture card feedback (see Safety Precautions below).

## Program Description

Hatch eggs from box.

## Safety Precautions

Scarlet & Violet is known to drop button inputs and can break the proper sequence of the program. It is therefore recommended to run this program with some level of supervising if you plan to run it for extended periods of time. 

Additional stability recommendations:
- putting your console in airplane mode
- restart the game after a hard save

## Program Setup

### Game Settings

1. Text Speed: Fast
2. Send to box: Auto
3. Nickname: Off
4. Auto-save: Off

### Party Setup

1. Have a Flame Body (or similar ability) Pokemon as your lead Pokemon.
2. If you have a cloned rider, place it in your 2nd party slot.
3. Leave the rest of the party slots empty.

### Box Setup

1. Place entire boxes filled with Eggs consecutively. It is okay to have a mix of Pokemon and Eggs. The only requirement is that each column has at least 1 Pokemon/Egg.
2. You must be on the first box of Eggs to hatch.

### Instructions

1. Cursor must be on Boxes when opening the menu.
   
   <img src="images/EggHatcher.png">
   
2. Fly to Zero Gate.
3. Start the program in the Change Grip menu.

## Options

If [**Tolerate System Update Menu (fast)**](/Wiki/Programs/NintendoSwitch/FrameworkSettings.md#tolerate-system-update-menu-fast) is selected, this program will try to bypass the system update window on game entry.

**Boxes to Hatch:** Select number of boxes to hatch. The optimal ratio of sandwich to box depends on the parent's compatibility and Egg Power level used.

**Step Count:** The number of steps needed to hatch the eggs. Look up the value on Serebii.

**Has cloned rider:** Check this box if you have a cloned rider in your 2nd party slot.

## Advanced Options

**Safety Coefficient:** If you note that the program frequently misses the last few eggs per column, increasing this number will extend the hatching time per cycle.

## Credits

- **Author:** Nymphea

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)
