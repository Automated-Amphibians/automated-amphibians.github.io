---
layout: content
---
### Feb 5th Mon
Field drive is indeed working
Tuned the intake only for it to die horribly    
Weighs in at roughly 75-80 lbs. We can add 40 lbs.

### Feb 4th Sun
Swerve drive software improved, not fixed - gyro orientation now suspected as problem.
Swerve fixed after gears thrown due to bad screws.
Arm breaks.
Acceleration improvements

### Feb 3rd Sat
Got chains installed, wiring completed, some arm issues addressed.

### Feb 3rd Fri
School closed, no work.

### Feb 2nd Thu
Chain box installed
One chain on the side installed
Wiring nearly completed

### Mar 1stth Wed
Wired the tension plate
More work on the chain box 
Worked on making sure that the robot would be legal 
Added surgical tubing for holding
Added U-bolts for hard stops

### Feb 28th Tue
Got the chain box (drives the arm), should have put it together, but did not -- ok it's harder than it looks
Got the sheet on, wiring started, and plastic sheet put together. We did get some wiring tied down as well.

### Feb 27th Mon
Vic found issues with the intake, we worked hard to fix them.

Took the tensioner plate off to add the steel cable.

Miguel and Nathan designed the chain box that will drive the arm.

### Feb 26th Sun (rare!)
Shoulder problems totally fixed, arms completed, intake resized and attached, tensioner plate installed

### Feb 25th Sat
Frame rebuild, arm attached, (shoulder problems mostly figured out)

### Feb 24th Fri
Frame nearly rebuilt

### Feb 23rd Thu
Started reading the instructions, watching the videos, geez that helps a lot. Frame rebuild worked on.
* Key Learnings:
    * Read the instructions!
    * Layout parts first!
    * Come up with a plan on how to assemble if one does not exist    

### Feb 22rd Wed - power outages
Frame complete - UH OH, as built, components will be outside of frame, need to rebuild
Intake finished, at home by Nathan

### Feb 21th Tue (long day)
More swerve driving, locking down components because they are flying off
Intake being worked on

### Feb 20th Mon (long day)
Bellyplate installed properly for first real driving
Swerve corrections
Grabbed sheet metal from alro, screws, lots of building 

### Feb 18th Sat
Wiring finally complete

### Feb 16th Thu
Frame done, start rewiring (not sure if this is the day we started)

### Feb 14-15th Tue/Wed
Bumpers were completed.

### Feb 13th Mon
Got new frame stuff, started on framing etc. 

### Feb 11th Sat
* Coding: Update constants in order to get the robot to drive straight, glue magnets in 
* Cutlist updated with correct instructions -- plan formulated for keeping everyone building - Nathan and Srinivas will coordinate
* Bumper: Fabric build/number application (mentor Chris from FF will assist) 

Swerve is mostly working. The motors move in the same direction, but when asked to do an in place rotation, it does the opposite of what it should do.

So, what could be happening is that we are literally driving backwards (likely) by using the turn encoder (which is the absolute encoder) and the drive encoders reversed. 

Incidentally, most swerve drives are left (counter-clockwise) is positive, right (clockwise) is negative. 

https://compendium.readthedocs.io/en/latest/tasks/drivetrains/swerve.html

Calibrated zero to the back, instead of the front. Corrected for this by reversing the turnign and drive motors. Tried calibrating the backwards
to 0.5, or 180 already, but didn't reverse the turning and drive motors appropriately. Do that and it should hopefully properly orient in place orientation.

Might be good to start with 
* What angle does the "spin in place" algorithm want?
* What direction does our current encoder work off of?

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
* Swerve coding
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
Sparkmax controllers wired into "temporary?" component ceiling

### Jan 25th?
Wood bellypan ceiling added

### Jan 21st
Chassis Frame completed.

First CAD model working

### Jan 14th
Swerves being built -- NEO motors ordered -- arrived Tuesday

### Jan 7th
Kickoff, game analysis.
