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

It'd be great to test the code off the robot before we test it on the robot.  How do aerospace companies handle this?  They must have some kind of aviation best practices.  In any case, we know they generally have working code prior to putting it on something that flies.

Would it be better to use the command and subsystem framework provided by the wpilib?  It seems like it'd result in more easily movable subsystems.  Moreover, it would make it so we could actually run unit tests - especially if we mock out the WPILib

It'd be really useful to have a tool that lists out all the active hosts on a network.  Or maybe just something that shows the full status of the local network at a glance - for example, DHCP vs autoconfiguration on the local IP address, whether MDNS has found the robot, whether the robot's up at its default address.

It'd be great to take advantage of the "vision calibration" opportunities offered at each event.  Furthermore, we should test from a multitude of angles, on every target on the field.  It would be really great to be able to do this with a laptop rather than the robot.

A logging utility would be super useful.  Nick has started it.

It might be nice to have a mock of the WPILib as a simpler standin for the simulator.  Just something to run the code and exercise certain paths.  It might be hard to make it useful without being a full simulator.  "Strongback" is such a library; we should look into that.

One thing we should test for and be vigilant for is the resetting of every state variable.  We had weird behavior in a practice match due to a variable that never got reset.

Would it be useful for the drive team to go and watch videos of their matches after the fact?  And ask questions like:
- What would have scored us more points?
- What mistakes did the other teams make?
