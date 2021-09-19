# Date Spam - Watt Farmer

## Program Description

WattFarmer will farm watts from a wishing piece beam. It requires activating the VS glitch.

This program runs at 6.9 seconds per fetch. This is about 1 million watts/hour at 2000/fetch.

<img src="images/DateSpam-WattFarmer.png" width="800">

### Setup of Settings

1. Text Speed: Fast
2. Casual mode: Off
3. System time: Un-synced
4. Y-Comm glitch must be active
   1. Verify glitch is active by checking for a "flash" when re-entering the game from the Home menu.
5. You must be offline.
6. Airplane mode must be off.

   > **Stability Recommendation:** Stand ***behind*** the den so that the beam is directly in front of your character. Sometimes, the program will miss a button press which causes the date-spamming to happen in the game instead of the Switch settings. This will cause the character to move downwards and away from the den if you’re not standing behind it.

### Instructions

1. You must be standing in front of a wishing piece den with watts collected.
2. Your location should be safe from getting attacked by wild Pokémon.
3. Start the program in the [Change Grip/Order Menu](/Wiki/Programs/NintendoSwitch/ChangeGripOrderMenu.md).

***

### Options

This program does not have the ability to avoid the system update window. Should the window appear while the program is running, the program will enter a safe do-nothing loop within the Switch settings.

### Fetch Attempts:
```
const uint32_t SKIPS            =   33334;
```
Perform this many fetch attempts. The only reason to set this number is if you’re also skipping to a den frame and you don’t want to overshoot. But be aware that this program isn’t intended to be an accurate date skipper. It may occasionally miss skips which can cause it to fall short.


### Periodically Save the Game:
```
const uint16_t SAVE_ITERATIONS  =   0;
```
If set to anything other than zero, the program will periodically save the game at the specified interval. In rare cases, the date-skipping can cause the game to crash, thus periodic saves can be enabled to reduce the amount of work that is lost.

***

## Advanced features

### Serial Output:

   > **THESE SETTINGS ARE ONLY APPLICABLE IF YOU ARE USING A SERIAL UART**

This program outputs the number of watt fetch attempts. This can be read by the serial programs.

***

## Troubleshooting

This program will not work if the system update window is present. Instead, it will safely enter a do-nothing loop within the settings.

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)


