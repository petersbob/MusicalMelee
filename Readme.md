# Musical Melee

## Creating music with Super Smash Brothers Melee

## What does it do?

This project allows you to customize the sounds coming out of Super Smash Brothers Melee. Information about what is happening on screen is pulled out from memory.

This data includes:
+ Character X position
+ Character Y position
+ Character stocks remaining
+ Character percent
+ Current stage
+ Jumps left

And much more.

### How was it built?

It is built using Python, [libmelee](https://github.com/altf4/libmelee), and [PureData](http://puredata.info/).

The Python program communicates with PureData over the [Open Sound Control (OSC)](http://opensoundcontrol.org/) protocol. Currently, the only Pure Data patch designed for an entire match was constructed using the synth "Automatonism" by Johan Eriksson (https://www.automatonism.com/).

It was built off of the work done by github user altf4 on his [SmashBot](https://github.com/altf4/SmashBot) AI project.

### What do I need to use it?

+ A mac or linux computer. The libmelee project is currently only working on mac and linux.
+ PureData, a visual programming language.
+ A custom version of the Dolphin emulator associated with libmelee. You can find that here: https://github.com/altf4/dolphin/tree/memorywatcher-rebased
+ A copy of Super Smash Bros. Melee v1.02 NTSC.
+ Lastly, you may want a gamecube controller and an adapter for use on your computer.

### I have that stuff, now what?

+ Install libmelee and the associated version of Dolphin.
+ Download or clone this project to your computer. 
+ Open of the PureData project, main.pd. You should hear sound right away. If you don't, navigate to the Media window and make sure DSP (Digital Signal Processing) is turned on. Verify that your audio settings in PD are correct as well.

+ Inside of the project folder, run
```
python3 MusicalMelee.py
```
+ Dolphin will start up.
+ Mute the sound. Config -> Audio -> Volume -> 0%
+ Start up Melee and the sound should begin to change once you start a fight.

### I can't get it to work!
MusicalMelee is still a young project and will likely be changing quite often. Please be patient as we update and fix issues.
