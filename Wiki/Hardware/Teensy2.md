# Hardware - Teensy 2.0 and Teensy++ 2.0

This section covers the required hardware for users who have chosen Teensy 2.0 or Teensy++ 2.0.


## Required Hardware

1. Teensy Board (**Choose one**)
   1. [Teensy 2.0](https://www.pjrc.com/store/teensy.html) 
      1. Sufficient for the programs in this project
   2. [Teensy++ 2.0](https://www.pjrc.com/store/teensypp.html) 
      1. More powerful and expensive than the Teensy 2.0

2. Mini-USB male to USB-A male cable or adapter. ([example](https://www.amazon.com/gp/product/B07QJTX59H/))

<img src="images/teensy2.jpg" height="100"> <img src="images/usb-a-to-usb-mini.jpg" height="100">

<img src="images/teensypp2.jpg" height="100"> <img src="images/usb-a-to-usb-mini.jpg" height="100">


The basic Teensy hardware setup will look something like this:

<img src="images/teensy-basic.jpg" height="350">

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
2. Board Connection (**Pick one**)
   1. Mini-Grabber to Male jumper wires ([example](https://www.amazon.com/gp/product/B08M5GNY47))
       > Easiest option, but item is hard to find
       <img src="https://raw.githubusercontent.com/PokemonAutomation/ComputerControl/master/Wiki/Hardware/images/serial-teensy2-mg.jpg" height="350">
       <img src="https://raw.githubusercontent.com/PokemonAutomation/ComputerControl/master/Wiki/Hardware/images/serial-teensypp2-mg.jpg" height="350">
   2. Solderless Hammer Headers ([example](https://www.adafruit.com/product/3662))
       > Fairly easy to install. Ensure you are getting _hammer headers_, they will have a bulge on the short side to hold the pins in place
       <img src="https://raw.githubusercontent.com/PokemonAutomation/ComputerControl/master/Wiki/Hardware/images/teensy2-hammer-0.jpg" height="350">
       <img src="https://raw.githubusercontent.com/PokemonAutomation/ComputerControl/master/Wiki/Hardware/images/teensypp2-hammer-0.jpg" height="350">
   3. Headers ([example](https://www.adafruit.com/product/2822))
       > Most difficult option! You will **need** to solder with this option. Please only pick it if you are comfortable soldering.

## Next Steps

Continue to the rest of [hardware tutorial](Hardware.md).

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)




