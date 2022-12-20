# Tera Raid AutoHost in Pokemon Scarlet and Violet
**CAPTURE CARD REQUIRED**

**Related Programs:**
- **Microcontroller:** [Tera Raid AutoHost](https://github.com/Vaedz7/Microcontroller/blob/master/Wiki/Programs/PokemonSV/TeraAutoHost.md) (this program)
- **Computer Control:** [Tera Auto-Host](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/AutoHost.md)

## Program Description

Automatically Host Tera Raids for Discord/Twitch without the use of a Serial Connection!

## Setup of Settings
### Board Setup
1. Follow Microcontroller guide by Pokemon Automation [here](https://github.com/PokemonAutomation/Microcontroller "here")
2. Download program(s) from **THIS REPOSITORY**
3. Copy and Paste ``TeraAutoHost_Core.c`` to ``CustomProgram_Core.c``
4. Compile CustomProgram.hex file for your board
5. Flash HEX file to your board

### In Game Setup
1. Stand in front of the Den you wish to host facing the crystal
2. Turn Auto Save **OFF**
3. Save incase of error
4. Have your first party Pokemon have an attacking move (Ideally something with at least 100 Damage) in the **FIRST MOVE SLOT**
5. Set Text Speed to **FAST**
6. Set your System Time to anything before 10 PM and after 1:59 AM

### Application Setup
1. Have your Discord WebHook URL ready and make sure the folder is located in ``Downloads`` and named ``TeraAutoHost``
2. Install Python from [here](https://www.python.org/downloads/ "here")
3. Open Terminal/Command Prompt and run the following commands ``pip install pytesseract``, ``pip install opencv-python``, ``pip install discord-webhook``, and ``pip install rich``
4. Now run ``cd Downloads/TeraAutoHost``
5. Then run ``python3 autohost.py``
6. Enter in WebHook URL
7. Select Video Capture Device
8. Add a description for users to see

### Starting the Program
1. Go to Change Grip/Order Menu on the Switch
2. Plug in your Board with the HEX file flashed
3. Press ``Start Program`` in the application

## Options
None

# Credits

- **Author:** Vaedz7


<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)

