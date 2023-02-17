# Hardware - Arduino Uno R3

This section covers the required hardware for users who already have the Arduino Uno R3.

**We only support Arduino Uno R3 as a legacy item.**

**If you are new to automation and do not already have an Uno R3, please buy either a Teensy or ProMicro.**

| **Setup** | **Est. Total Price** |
| --- | --- |
| Arduino Uno R3 | Not worth your time and money.<br>Not worth *our* time to help you debug it. |

***(You have been warned.)***

Why we do not support it:
1. The Uno R3 and its knock-offs do not have enough memory or flash storage to run all the programs in this project.
2. Many of the Uno R3's that are sold cannot be put into DFU mode. Therefore you cannot program them and they cannot be used.
3. Driver support for the Uno R3 is very flaky. Sometimes it works out-of-box. Other times, it requires manual driver installation.
4. The Uno R3 is complicated to use as it requires manually shorting pins and multiple actions on the computer. By comparison, [Teensy](Teensy2.md) has a button that does all this.

## Required Microcontroller Hardware

1. [Arduino Uno R3](https://store.arduino.cc/usa/arduino-uno-rev3)
2. USB-B male to USB-A male cable. ([example](https://www.amazon.com/Monoprice-1-5-Feet-24AWG-Plated-105436/dp/B009GUVZOK))

<img src="https://raw.githubusercontent.com/PokemonAutomation/SwSh-Arduino/master/Documentation/Tutorials/images/uno-r3.jpg" height="200"> <img src="https://raw.githubusercontent.com/PokemonAutomation/SwSh-Arduino/master/Documentation/Tutorials/images/usba-usbb.jpg" height="200">

3. Switch Lite users will also need a USB hub or portable dock. ([example](https://www.amazon.com/gp/product/B07JK9DFKH))

> The Switch Lite does not have a USB-A port. Therefore you need either an adapter or a hub to connect the microcontroller. A charging hub or dock is required to simultaneously charge and use the microcontroller.
>
> Note: even on a dock, Switch Lite cannot output video over HDMI.

## Serial Hardware for Computer-Controlled Programs

If you only need microcontroller-only programs, skip this section.

1. Serial Board (**Pick one**)
   1. UART Cable ([CP210x controller](https://www.adafruit.com/product/954)) Adafruit UART cable is not the cheapest, but it is the most beginner-friendly.<br><br>
      ***DO NOT get the Prolific (PLxxxx) controllers.* They do not work and they are explicitly blocked in the program.**<br><br>They are cheap because they do not work. If you buy it anyway, you will be wasting your time and money.<br><br>**YOU HAVE BEEN WARNED!**<br><br>
   2. CP210x board ([4 for $8](https://www.amazon.com/gp/product/B07T1XR9FT)) | ([2 for $8](https://www.amazon.com/gp/product/B07D6LLX19/)) | ([1 for $8](https://www.amazon.com/dp/B072K3Z3TL))
      >  If you are experienced (or confident), these are some cheaper alternatives which also work. These may require a trivial amount of extra wiring.
2. Jumper Wires ([example](https://www.amazon.com/dp/B07GD2BWPY))

<img src="https://raw.githubusercontent.com/PokemonAutomation/ComputerControl/master/Wiki/Hardware/images/uart-uno-0.jpg" height="600">

## Next Steps

Continue to the rest of [hardware tutorial](Hardware.md).

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)



