# Egg Combined

**Related Programs:**
- **Microcontroller:** [Egg Combined](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSV/EggCombined.md) (this program)
- **Microcontroller:** [Egg Hatcher](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSV/EggHatcher.md)
- **Microcontroller:** [Egg Fetcher](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSV/EggFetcher.md)
- **Computer Control:** [Egg Fetcher](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/EggFetcher.md)
- **Computer Control:** [Egg Hatcher](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/EggHatcher.md)
- **Computer Control:** [Egg Autonmous](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/EggAutonomous.md)

The microcontroller and computer-control versions of this program are conceptually similar, with the microcontroller version being less error tolerant without capture card feedback (see Safety Precautions below).

## Program Description

Collect eggs in picnic by making Egg Power sandwiches, then hatch eggs from box.

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

1. If you have a cloned rider, place it in your 2nd party slot.

### Box Setup

1. Place a Flame Body (or similar ability) Pokemon on the first slot in the box to the left of the initial egg collection box and leave the left two columns empty. Parents will be deposited in this box after fetching eggs at picnic.
2. Current and consecutive boxes to the right have sufficient spaces to deposit eggs.

### Picnic Setup

1. Have sufficient Ham and Butter to make the sandwiches (Sweet Herba Mystica as well if selected).
2. If using Sweet Herba Mystica, have Recipe #3 unlocked (given by NPC in most sandwich shops).
3. Having completed the Picnic/Sandwich tutorial.
4. (Optional) Consider bringing smaller Pokemon if the program keeps interacting with Pokemon instead of the basket.

### Instructions

1. Cursor must be on Picnic when opening the menu.
   
   <img src="images/EggFetcher2.png">

2. Fly to Zero Gate.
3. Start the program in the Change Grip menu.

## Options

If [**Tolerate System Update Menu (fast)**](/Wiki/Programs/NintendoSwitch/FrameworkSettings.md#tolerate-system-update-menu-fast) is selected, this program will try to bypass the system update window on game entry.

**Use Sweet Herba Mystica:**
- Yes: Egg Power 2 (1 Ham + 1 Butter + 1 Sweet Herba Mystica)
- No:  Egg Power 1 (1 Ham + 1 Butter)

**Maximum amount of sandwiches to make:** The maximum amount of sandwiches the program should make.

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
