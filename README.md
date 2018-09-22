# Nerf Iron Dome
![Turret](https://github.com/brianlevis/nerf-iron-dome/raw/master/turret.jpg)
## Contributors
[Brian Levis](https://github.com/brianlevis) • [Luciano Vinas](https://github.com/lucianovinas) • [Andrew Chan](https://github.com/theandrewchan)
## Summary
The aim of this project is to build a nerf turret that can do cool stuff. Cool stuff might include:
* Targeting a moving object (tennis ball?)
* Recognizing faces
* Being remote controlled
* Guarding an object
* Reenacting [this scene](https://www.youtube.com/watch?v=mrXfh4hENKs) from RoboCop

## Status
The turret has been constructed, and may be controlled via a USB Xbox 360 Controller. It's electronics are ~~spaghetti~~ no longer spaghetti.
The turret can track and attack an object of a certain color (defined as a range of HSV values) and size, such as a green tennis ball or maroon sweatshirt. Even when the target is reliably identified however, tracking is not terribly smooth.
## TODO
Software:
* Improve object tracking techniques
* Add better object recognition (faces, clothes)
## Credits
Turret base inspired by Britt Michelsen's [Nerf Vulcan Sentry Gun](http://www.instructables.com/id/Nerf-Vulcan-Sentry-Gun/), Nerf RapidStrike [teardown guide](http://torukmakto4.blogspot.com/2013/10/standard-rapidstrike-illustrated-guide.html),
[xboxdrv python wrapper class](https://github.com/FRC4564/Xbox)
## Tech
### Hardware
Nerf RapidStrike with pusher and flywheel motors hooked up to 7.5V 100W power supply and 5V relay module. Super high torque HS-805BB servos hooked up to 6V 18W power supply. Arduino controls all actuators, and communicates over serial with Raspberry Pi. Raspberry Pi Camera v2 mounted on top of gun. Possibly will be mounted on drum tripod.
### Software
[Python Connector Design](https://docs.google.com/document/d/1Gke5QFeYasZ8_wYOghZAU99f_aja3h15VcXeIRREn2o/pub)
