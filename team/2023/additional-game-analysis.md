---
layout: content
---
### Field Layout
<a href="2023FRC_Cheatsheet_Print-01.png"> ![](2023FRC_Cheatsheet_Print-01.png)</a>

### Use WPILib swerve code?
https://www.chiefdelphi.com/t/moving-swerve-code-from-sds-to-wpi/418993/4

### Balancing Robot Code
https://www.chiefdelphi.com/t/warning-to-everyone-working-on-auto-balance/422460/8

https://github.com/GOFIRST-Robotics/Ri3D-2023/blob/main/src/main/java/frc/robot/commands/BalanceOnBeamCommand.java

https://www.youtube.com/watch?v=2D3LOCGfEc4

https://www.mathworks.com/help/control/ug/two-degree-of-freedom-2-dof-pid-controllers.html

### How does the match look from the drivers perspective?
Also read 6.1.3

#### Answer 1
You're staged in a queueing area right behind the driver area. After the preceding match ends, those drivers pick up their stations and you can put yours down, while the rest of the drive team gets the robot placed on the field and turned on. You can select auto modes during that time. You can watch some of the top-down stream videos to watch what all happens between matches.

You're standing behind the line for auto. After auto ends, there's a bell, and the drivers can step forward and pick up controllers. The field automatically manages all the modes and stuff, so auton will just run when everything is ready and the field/GA counts down. Driver station is often just a tray with a laptop, charger, and controller/gamepad sitting on it. 

https://www.youtube.com/watch?v=YwFJ4Tk3wKM
https://www.youtube.com/watch?v=69hDwCe8smE&t=77s
https://www.youtube.com/watch?v=fBtGWijXizI
https://www.youtube.com/watch?v=riPvXtiG75w

#### Answer 2
I'll try to give a bit of a walk through of what a match looks like setup-wise from the drive team. 

During each event, you'll see that you have a match via your provided schedule, and you'll start bringing the robot and drivers station (we just used a laptop and two playstation controllers) over to the queueing area before it. This will vary by event, but it will be well labeled and pointed out to you in the driver's meeting (more info later). 

There will be a volunteer with a clipboard called the queuer, who you will check in with by just saying your team number. You'll wait in queue until it's your time to load onto the field, which will be indicated by the queuer. From here, our drive team split up. 

For loading the Robot on the field: Three drive team members carried the robot from the cart onto the field, set it down on the carpet, turned it on, and loaded the game piece.

For drivers station (me!): I took the laptop and controllers over to the driver's station (shelf behind the glass), plugged in the controllers and field ethernet cable, turned on the laptop and booted up Drivers Station (DS). Always close out of DS after every match, it prevents Issues™️. 

After the robot is set on the field, the entire drive team met me behind the glass, and the auto routines were selected. This could have been done by me at any point after DS was loaded, to clarify.

After we established that the laptop and robot are connected, we set the controllers in an easily grab-able location on the shelf for when Teleop starts. At this point, the Game Announcer will probably start running through the teams and robots. If at any point during this process you have technical issues, you can flag over an FTA or FTAA who will help you (if you're not connected soon, they'll most likely just show up anyways).
For the match to start, all drive team members must be behind the line (tape on the ground), then the Refs will start giving thumbs up to the Head Ref, and the match will begin! Auto routines will be initiated by the field, so you don't need to do anything for that. This year is different with when you can grab the controllers (review the rules carefully for that), but I believe you should be able to have them in hand when teleop starts. There will be an auditory and visual cue to indicate teleop start, and you're off to the races. 

Once the match ends, its the reverse process: Close DS and unplug the field ethernet while other members start taking the robot off the field. Your technician will have the robot cart during the match and will be directed to the unloading side of the field, typically the side with the scorekeeper's table, right before the match ends.
One thing about all this: There will be a drive team meeting the first morning of each event where one of the Volunteers (Head Ref iirc) goes over general logistics and things specific to each venue. If at any point you are confused or want clarification, ask! Everyone wants you to have fun and knows what its like to go to your first comp, so they'll be very friendly.

VERY IMPORTANT TO GOTO DRIVER MEETING


### Discussion of scouting

For comparison sake, this is what I think Frog Force is going to be looking for when we select our alliance partners (and the top teams at your events should be similar).  At this point, we don't care if a team scores only one kind of piece, although diversity is always better.  There are 6 spots to score cubes and 12 to score cones, and 9 where either one can be scored.  Very good teams might be scoring 8-10 in a match, so nobody should run out of spots to score. I think we optimistically calculated every robot can technically score as many as 7-8 during teleop, but even if everyone scores one during auton, there's no shortage of space. I am curious to see how many single game piece type robots there are, and what type it will be. I'm sure if the everybot is only one type (which seems logical), then that could dominate.

1. The captain (hopefully us).  Can do everything.  Score at least two pieces in autonomous and balance.  If we're capable of scoring more than two, at least one of our partners needs to be able to balance in auton reliably.  Can score both game pieces at all levels, as many as possible.  Can triple-balance at the end.
2. First pick.  As close to a copy of the captain as possible.  We want to team up the two best scoring robots and win.  We'd be looking for a 2-piece autonomous, with or without the auton balance, depending if the captain is capable of using that time for another piece (If all we can ever do is two, then we'll probably just do those two and balance... we tend to not trust other teams if we're confident in ourselves).  Preferably on the skinnier side so we can easily triple-balance at the end.
3. Second pick.  This robot is probably going to play defense during the playoffs unless they're just a phenomenal scorer.  Traffic jams at the loading station and the Community make it best to not always have three scoring bots when two of them are high-powered.  Our first criteria is swerve, if possible.  Since the first two robots will be doing 2-piece autons, we probably just want this one to score their pre-load and balance.  If they've demonstrated that they can leave the community for the mobility points, without going so far that they interfere with the pieces on the floor, they can do that, but most likely we don't even want them to leave the Community, just score and balance.  They'll play defense during teleop most likely.  Be skinny enough to triple-balance.
4. What about a runner robot?

> This gets me into a whole different conversation that I could write another book on.  The short version is, for the playoffs the alliance captain is generally recognized as the leader of the alliance.  They likely drafted each team with a role in mind for them.  So it's not uncommon for the third robot to be drafted "to play defense", and it's appropriate to make that "demand".  The captain may (and should) ask for input, but in the end it's their call.  

> There are no such expectations in the qualification matches.  It doesn't matter if it's a rookie team and a Hall of Fame team, everybody should have input on the plan.  Don't let teams "tell" you what you're going to do during quals.  A lot of times teams are told to "play defense" as a way of saying "stay out of our way."  I can totally see this. (hopefully we get there and make use of this advice)  If it makes sense for you to play defense, they should be able to explain why, maybe using numbers from their scouting data.  And even if they do show you "you only score two pieces, and we think you could slow down the other team by a larger margin than that", you don't have to do it, although that tends to make teams mad at you and if they're one of the top teams at the event that kills your chances of them picking you.  But if you think you've fixed your intake that hasn't been working and you really need to try it, tell them that.  Maybe you agree that you'll try one or two pieces, and if t's not working in 15 seconds you'll abandon it, but if it's working you want to keep scoring, and you can agree that the faster scoring bot will get the right-of-way in the loading and scoring zones, or whatever.  The bottom line is you can listen to their advice, but you don't have to.  Just make sure to do what you say you will.  Teams that agree to a plan, even reluctantly, and then don't follow it end up on "do no pick" lists. Kinda get that.