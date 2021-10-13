# Microcontroller Programs - Hardware Guide

This is the guide for buying and setting up the hardware for the microcontroller programs.

If you already have the hardware, skip ahead to the software tutorial.
- [Software Tutorial](/Wiki/Software/README.md)

## Pick Your Hardware

(insert descriptions)


### Teensy 2.0 or Teensy++ 2.0:

<img src="images/teensy-basic.jpg" height="350">

Teensy 2.0 is the recommended controller for beginners. It is the easiest to use with the most user-friendly software and a push button to flash it.

Teensy++ 2.0 is just as easy, but is overkill. Don't get it unless it's almost the same price as the Teensy 2.0.

The total cost for each setup is approximately

| **Controller** | **Est. Total Price** |
| --- | --- |
| Teensy 2.0 | $25 USD |
| Teensy++ 2.0 | $35 USD |


### Pro Micro:

<img src="images/pro-micro-basic.jpg" height="350">

The Pro Micro is recommended for experienced users. It is harder to use, but is cheaper especially in volume.

| **Setup** | **Est. Total Price** |
| --- | --- |
| 1 x Setup | $15 USD |
| 4 x Setup | $35 USD |

### Arduino Uno R3 (not recommended):

<img src="images/uno-r3.jpg" height="200">

The Arduino Uno R3 is not recommended at all. While we technically still support it, it is officially deprecated.

Why is Uno R3 not recommended?

1. The Uno R3 and its knock-offs do not have enough memory or flash storage to run all the programs in this project.
2. Many of the Uno R3's that are sold cannot be put into DFU mode. Therefore you cannot program them and they cannot be used.
3. Driver support for the Uno R3 is very flaky. Sometimes it works out-of-box. Other times, it requires manual driver installation.
4. The Uno R3 is complicated to use as it requires manually shorting pins and multiple actions on the computer. By comparison, [Teensy](Teensy2.md) has a button that does all this.

We do not recommend continuing with the Arduino Uno R3 unless you already have one sitting around. Do not go and buy one.

In the future we will likely drop support for it completely as it has become a maintenance and tech-support burden for us. **Likewise, we no longer provide tech-support for Arduino Uno R3 unless you demonstrates computer competency and have at least a bachelor's degree in electrical engineering.**

| **Setup** | **Est. Total Price** |
| --- | --- |
| Arduino Uno R3 | Not worth your time and money.<br>Not worth *our* time to help you debug it. |

### Other Controllers:

While not officially supported, the Arduino Mega 2560 R3 and the Arduino Leonardo have been tested to work using either the Teensy 2.0 or Pro Micro .hex files since they all use the same ATmega32u4 processor. The only thing that won't work are the LEDs since the I/O ports are different.

Do not use the other Teensy models (LC, 3.x, 4.x, etc...). They are ARM-based boards which we do not support at this time.


## Next Steps

Continue to the guide for the device you have chosen:

- [Teensy 2.0 or Teensy++ 2.0](Teensy2.md)
- [Pro Micro](ProMicro.md)
- [Arduino Uno R3 (deprecated)](ArduinoUnoR3.md)

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)
