If we do another practice robot:
* Think about trying to plan the post-season meeting schedule before the build season wraps up
* Consider and discuss a "programming season" which overlaps with the build season.  For example, start the software 2 weeks into the build season, so the programmers have energy for another 2-4 weeks of programming after stop build.

We could iterate on PID tuning and auto moves a lot more quickly if all the relevant parameters were stored in JSON files or something on the file system, rather than constants in the code.

What is stopping us from using the PID loops on the Talons?  Does it not work in follower mode?

Would be super amazing to have some form of Built-in TEst.  Like maybe:
* Pressure sensor in the pneumatics
* Encoders on all the things

Would be really great just to have a rock solid motion control module for each drive pod.  Would be super cool to have a test stand for a motor to push against.

We could feasibly design the robot's software in advance of the build season, and then write modules to support features that are likely to be present in the game.  Taken to the extreme, you could write a meta-language in which you define the robot's behavior in config files.

Testing.

Would it be better to use the command and subsystem framework provided by the wpilib?
