---
layout: content
---
### Feb 11th Sat
* Coding: Update constants in order to get the robot to drive straight, glue magnets in 
* Cutlist updated with correct instructions -- plan formulated for keeping everyone building - Nathan and Srinivas will coordinate
* Bumper: Fabric build/number application (mentor Chris from FF will assist) 

Swerve is mostly working. The motors move in the same direction, but when asked to do an in place rotation, it does the opposite of what it should do.

So, what could be happening is that we are literally driving backwards (likely) by using the turn encoder (which is the absolute encoder) and the drive encoders reversed. 

Incidentally, most swerve drives are left (counter-clockwise) is positive, right (clockwise) is negative. 

https://compendium.readthedocs.io/en/latest/tasks/drivetrains/swerve.html

I've calibrated zero to the back, instead of the front. We've corrected for this by reversing the turnign and drive motors. I tried calibrating the backwards
to 0.5, or 180 already, but I didn't reverse the turning and drive motors appropriately. Do that and it should hopefully properly orient in place orientation.

### Feb 10th Fri
* More pieces of the gamespec cut

### Feb 9th Thu
* Swerve working, need to get offsets properly completed
* Attached bumper holders
* Cut first pieces of gamespec/mechanism

### Feb 8th Wed
* Struggled with Swerve
* More CAD work?

### Feb 7th Tue
* Try to keep everyone busy - can't even remember what we managed to get done
* Let other mentors work on swerve coding
* Organized and went through parts list -- ordered couple missing items

### Feb 6th Mon
* More work done on cad to figure out how mechanism will be placed on top -- widened mechanism
* Absolute encoder and motor controllers mapped to correct values, first attempt at driving straight
* Handed off bumper to Chris for fabric work

### Feb 4rd Sat
* More bumper work -- ready to mount
* Battery and other parts moved to top
* Work done on cad to figure out how mechanism will be placed on top
* Added absolute encoder

### Feb 3rd Fri
* More bumper work -- foam placed

### Feb 2nd (thu)
* Bumper work?

### Feb 1st (wed)
* Electronics -- velcro/screw everything down
* First test with new Swerve library
* Cut baseplate?

### Jan 31st
* Bumper screw mounts placed?
* Swerve motors and motor controllers tested and CAN properly wired
* Bellypan/ceiling design CAD work

### Jan 30th
* Electronics: Update Roborio software with latest image
* Electronics: Program Radio
* Bumper: Work done
* Admin: Write letter for magna

### Jan 28th
Loaded firmware for Sparkmax controllers, finished wiring PDP (16-20x ferrule + anderson powerpole connectors made), velcroed on PDP, Sparkmaxes

### Jan 27th
Sparkmax controllers wired into "temporary?" bellypan ceiling

### Jan 25th?
Wood bellypan ceiling added

### Jan 21st
Chassis Frame completed.

First CAD model working

### Jan 14th
Swerves being built -- NEO motors ordered -- arrived Tuesday, 

### Jan 7th
Kickoff, game analysis.






