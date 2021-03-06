# Calibrating Unattended Shiny Hunting 

CALIBRATION IS A REQUIRED PART OF GETTING THIS PROGRAM TO WORK PROPERLY

## How to Calibrate:

Calibration involves setting the delay so that the program runs away from the encounter shortly after the battle menu appears. To aid in this process, the program will turn on the LEDs on the device the moment it starts the run-away sequence.

While the exact timing recommendations will vary by program, but for the most part when calibrated correctly:
1. When the encounter is not shiny, the following happens
   1. The LEDs should turn on ***0.5 – 1.5*** seconds AFTER the battle menu appears.
   2. The program will run away from the battle.
2. When the encounter is shiny, the following happens
   1. The LEDs should turn on ***0.5 – 1.0*** seconds BEFORE the battle menu appears.
   2. The program will _not_ run away and will instead trap itself in the summary of your Pokémon.

To check your calibration, you need to test both cases and observe when the LEDs turn on. #1 can be tested by running the program as instructed above and observing the timings. In order to test #2, you need to simulate encountering a shiny. There are two main ways to do this:

### **Method 1:**
**NOTE: This method is less convenient to set up, but more convincing to first-time users.** 
1. Replace your non-shiny lead Pokémon with a same species shiny that satisfies all requirements listed below
> Lead Pokemon Requirements
> * Your lead Pokémon must be able to run away. (faster or holding Smoke Ball)
> * Your lead Pokémon must not have high happiness. The in-battle shaking and dialog adds timing variation.
> * You must turn off your lead Pokémon following you. Following will cause happiness to increase enough to shake in battle. You can do this by talking to the boy in Freezington.
> * Since different Pokémon have different animation lengths, it is strongly recommended to use a shiny-lead of the same species as your intended non-shiny lead.
2. Use a stopwatch to time from when the battle starts (screen goes black), to when the battle menu pops up
> EX: Calibrate with a shiny Magikarp if running the program with a normal Magikarp. When you test the two cases (non-shiny and shiny), observe when the LEDs turn on. **Use a stop watch!**
> - If the LEDs turn on too early, you should increase the delay.
> - If the LEDs turn on too late, you should decrease the delay.
> - Each tick is 8 milliseconds (125 ticks per second). So use this to calculate the size of your adjustments.
3. Increase / Decrease delay per above notes
> - Ex: If the LEDs turn on 0.5 second too early, increase the delay 63 ticks
4. Check that program locks on a non-shiny target mon
5. Swap out your shiny lead for the non-shiny lead that fulfills the requirements in item #1
6. Run program and check later for a shiny lock

### **Method 2:**
1. Run the program and see if it _runs_ from non-shiny target mons (i.e.; searching for Regis)
> Lead Pokemon Requirements
> * Your lead Pokémon must be able to run away. (faster or holding Smoke Ball)
> * Your lead Pokémon must not have high happiness. The in-battle shaking and dialog adds timing variation.
> * Your lead Pokémon must not be shiny.
> * You must turn off your lead Pokémon following you. Following will cause happiness to increase enough to shake in battle. You can do this by talking to the boy in Freezington.
2. Once you have confirmed that you run from non-shinies, reduce the delay by 250 ticks.
> Reducing by 250 ticks simulates the 2.0 second delay from an actual shiny encounter. This method is easy and reliable, but less convincing to first-time users.
3. Run program again to confirm program locks on a non-shiny target mon
> If this locks, it proves the calibration will lock on a shiny target mon
4. If #3 is true; increase the delay back up 250 ticks
5. Run program and check later for a shiny lock

## Explanation of why this is required

Calibrating an unattended shiny hunting program involves changing a specific delay such that the run-away (called "branching") sequence happens shortly after the battle menu appears.

> Each program has a different name for this delay, so check the section for that specific program. But they all serve the same purpose – to tell the program when to run away from the encounter.

The programs come with a default delay, but you will need to change it:
- The Regi and Regigigas programs will probably work out-of-box for most people. The timings are very consistent across Switches.
- The Strong Spawn program may require large timing changes depending on the weather and any activating abilities.
- The Swords of Justice program is the most difficult to calibrate because it has large timing variations. It may not even be possible on systems with too high variability.

**When correctly calibrated:**
- If the encounter is not shiny, the program will run* from the battle and move on to the next encounter.
> *The Regigigas program does something different since you can't run from it.
- If the encounter is shiny, the program will trap itself inside the Pokémon menu. This allows you to manually back out and fight the shiny Pokémon.


***

# Troubleshooting

### Delay Drift:

Over time, delays can drift. If you have properly calibrated your delay to a specific value, it may no longer work after a sufficient amount of time (days). This is because the Switch can slow down or speed up with time due to environmental factors.
Thus, you will need to check your calibration every day or so to make sure it still works. It usually suffices to just watch a few encounters and pay attention to when the light turns on. Only if things are off should you bother with checking the shiny encounter case to make sure it still locks with the recommended time margin.

### Failure Cases:
- If the program traps on a non-shiny _[false positive]_
  - This happens if the program tries to run too early. It usually means the delay is too low.
- If the program runs from a shiny _[false negative]_
  - This happens if the program runs too late. It usually means the delay is too high.
- The program occasionally attacks a non-shiny instead of running from it
  - This happens if the run-away sequence was partially cut-off before the battle menu appeared. It usually means the delay is too low.
- The program attacks a shiny instead of locking it
  - This is the same as the previous bullet and is extremely rare since it requires a shiny encounter. It usually means the delay is too high.

These failure cases mean that if you come back and see your Switch trapped in the summary screen, it doesn't guarantee that the encounter is shiny. This is actually quite common depending on the program and the quality of the calibration.

***

### How it works

Unattended shiny-hunting programs are new to the Crown Tundra DLC (though the concepts involved have been found to work on the base game as well).

The idea with unattended programs is to repeatedly reset for a shiny encounter and then automatically stop when a shiny is found.

But how is this possible? There is no feedback. The device can't tell if there's a shiny since it can't see the screen or hear sounds.
It is in fact possible. The trick is to abuse the fact that the shiny animation adds a 2 second delay to when the battle menu appears. Thus you can use these 2 seconds to swallow a sequence of button presses that would cause a branch in the state sequence such that one branch resets, while the other branch does not. For most of the unattended shiny-hunting programs, this sequence is to run from the encounter.

Thus, the key is to run from the non-shiny encounter within 2 seconds of the battle menu appearing. If the encounter is shiny, this does not happen and the program proceeds to trap itself inside the summary of your Pokémon thereby stopping the resets.

Demo Video: https://cdn.discordapp.com/attachments/755635697737531544/772244388109090817/ShinyTerrakion.mp4

*The difficulty of the unattended shiny hunting programs is that the "branching sequence" needs to happen during that 2 second window. Due to differences and variations between different Switch systems and environments, the delays to when the battle menu appears will be different. There is no one setting that fits all. Therefore, all unattended shiny-hunting programs require calibration to work properly.*





<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)





