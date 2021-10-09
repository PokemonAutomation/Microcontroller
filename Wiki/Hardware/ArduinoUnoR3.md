# Hardware - Arduino Uno R3

This section covers the required hardware for users who already have the Arduino Uno R3.

**We only support Arduino Uno R3 as a legacy item.**

**If you are new to automation and do not already have an Uno R3, please buy either a Teensy or ProMicro.**

***(You have been warned.)***

Why we do not support it:
1. The Uno R3 and its knock-offs do not have enough memory or flash storage to run all the programs in this project.
2. Many of the Uno R3's that are sold cannot be put into DFU mode. Therefore you cannot program them and they cannot be used.
3. Driver support for the Uno R3 is very flaky. Sometimes it works out-of-box. Other times, it requires manually driver installation.
4. The Uno R3 is complicated to use as it requires manually shorting pins and multiple actions on the computer. By comparison, [Teensy](Teensy2.md) has a button that does all this.

## Required Hardware

1. [Arduino Uno R3](https://store.arduino.cc/usa/arduino-uno-rev3)
2. USB-A male to USB-B male cable. ([example](https://www.amazon.com/Monoprice-1-5-Feet-24AWG-Plated-105436/dp/B009GUVZOK))

<img src="https://raw.githubusercontent.com/PokemonAutomation/SwSh-Arduino/master/Documentation/Tutorials/images/uno-r3.jpg" height="200"> <img src="https://raw.githubusercontent.com/PokemonAutomation/SwSh-Arduino/master/Documentation/Tutorials/images/usba-usbb.jpg" height="200">

**Switch Lite users will also need:**

1. A USB hub or portable dock. ([example](https://www.amazon.com/gp/product/B07JK9DFKH))

> The Switch Lite does not have a USB-A port. Therefore you need either an adapter or a hub to connect the Teensy. A charging hub or dock is required to simultaneously charge and use the Teensy.
> 
> Portable docks will work for the Switch Lite. It will just not be able to output video over the HDMI.

## Optional Hardware

* If you are a heavy user, then it is strongly recommended to get a USB-A male-to-female cable with a power switch on it. ([example](https://www.amazon.com/gp/product/B07T9BRNHW))

* If you intend to change programs very often and will be running the Switch next to a computer, then you will want a USB switch. ([example](https://www.amazon.com/gp/product/B006Z0Q2SI)) These are like USB-only KVM switches. In fact a regular KVM switch will also work. With this, you no longer have to constantly plug/unplug USBs which will eventually wear them down.

Heavy users in general will probably want to upgrade to using the [computer-control programs](https://github.com/PokemonAutomation/ComputerControl) instead.

## Next Steps

Continue to the [software tutorial](/Wiki/Software/README.md).

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)



