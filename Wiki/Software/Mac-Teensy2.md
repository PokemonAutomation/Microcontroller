# Tutorial - Mac - Teensy 2.0 and Teensy++ 2.0

This section will walk you through the entire process of setting up your Teensy on a Mac computer.

At this time, the HexGenerator program on Windows is not yet available for Mac or Linux.

## Step 1: Acquire the Hardware

Make sure you have the hardware:

* [Hardware - Teensy 2.0 and Teensy++ 2.0](/Wiki/Hardware/Teensy2.md)

## Step 2: Install Homebrew and AVR

1. Install homebrew: https://brew.sh/
2. Install AVR:
    1. Run `brew tap osx-cross/avr`.
    2. Run `brew install avr-gcc`.
    3. Run `brew install avrdude`.
3. Install fzf: `brew install fzf`

## Step 3: Download Teensy Loader

Download [Teensy Loader](https://www.pjrc.com/teensy/loader_mac.html).

Direct download link: https://www.pjrc.com/teensy/teensy.dmg

## Step 4: Download the Arduino Programs

Download the latest version of our Arduino programs from [here](https://github.com/PokemonAutomation/Microcontroller/releases).

(The link should look like something like `PA-NativePrograms-0.x.x-xxxxxxxx.zip`)

If you get a virus or malware warning, ignore it. These are known false positives. If you don't trust us, the source code is in this repo.

Once you have downloaded the package, unzip to somewhere you can access later.

## Step 5: Configure the program.

This step isn't needed for the TurboA example here, but is for nearly every other program.

1. Navigate into the `NativePrograms/NintendoSwitch` folder.
2. Open `TurboA` with a text editor.
> We recommend starting with "Turbo A"  as it is the simplest program. If you are able to get this running, it is easier to troubleshoot the other programs.

Normally you will see a bunch of options that can configured. But TurboA has nothing.

3. After you have made your changes, save the file.

See the documentation for the respective program for a description of all the options.

## Step 6: Generate a .hex file.

1. Open Terminal
2. Type `bash ` (with a trailing space!) Do not hit enter after entering this.
3. Drag from finder the "00-BuildAllUnix.sh" script into the Terminal Window.
4. Press enter.

This will build every single program in the package. As of this writing, there is no easy method to build that is more targeted. If you are confortable with makefiles and command lines, you can directly use the makefile.

## Step 7: Flash the .hex into the Teensy.

1. Run the Teensy Loader program that you downloaded earlier.
2. Click the purple file icon and browse for the .hex that was created in the previous step.

<img src="images/tutorial-windows-teensy-2.png">

3. Plug the Teensy into your computer.
4. Press the white button on the Teensy. You may need to wait for Windows to install drivers.

At this point, two green arrows should show up in Teensy Loader.

<img src="images/tutorial-windows-teensy-3.png">

5. Click the left arrow. This flashes the program into the Teensy.

<img src="images/tutorial-windows-teensy-4.png">

6. Unplug the Teensy from your computer.

## Step 8: Setup and run the program!

1. On your Switch, enter the game and navigate to somewhere you want to mash A in front of (such as the digging duo).

<img src="images/digging-duo.jpg" height="400">

2. Navigate to the grip menu without closing the game. This disconnects all controllers from the Switch so that the Teensy can take over.

<img src="images/grip-menu.jpg" height="400">

3. Plug the Teensy into your Switch (or the dock that's attached to it).

The program should now begin running. It will flash its light for a few seconds, then it will connect to the Switch and navigate its way back into the game. After a brief pause, it will start mashing A.

**Usage Notes:**

- To stop the program, simply unplug the Teensy at any time.
- Do not change video output or mess with the HDMI. These can cause the program to Switch to freeze for multiple seconds and break the program. If you want turn off the TV, do it *before* you start the program.

## Other Programs

You now know how to run TurboA - the most basic of the programs. You can choose any of the other programs and repeat steps 5-8.

- [Program List](/Wiki/Programs/README.md)

It is important to read the manual for a program before you use it. Each program has a different set of instructions and startup conditions.
You can find the manual for a program by clicking on the "Online Documentation" link.

## Computer-Control

As of this writing, Computer-Control programs are only supported for Windows. But feel free to browse the [Computer-Control tutorial](https://github.com/PokemonAutomation/ComputerControl/tree/master/Wiki/Hardware/README.md) anyway if you decide to switch to Windows.


<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)


