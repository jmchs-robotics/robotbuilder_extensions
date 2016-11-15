# robotbuilder_extensions

RobotBuilder works very well for creating robot programs that just use WPILib for motors, controllers, and sensors. But for teams that use custom classes, RobotBuilder doesn't have any support for those classes, so a few steps need to be taken to use them in RobotBuilder.

Custom components all go in $USER_HOME/Robotbuilder/extensions. On Linux and Mac, $USER_HOME will be /Users/yourusername/. On Windows, it will be C:\Users\yourusername\

Here is a link that describes how to create these sorts of extensions.
https://wpilib.screenstepslive.com/s/4485/m/26402/l/470258-adding-custom-components

## Status of the extensions

### RobotDrive6

This is mostly done, however there is no constructor for RobotDrive in the wpilib that takes 6 motors. I will be pushing that change up to the wpilib developers.

### TimedCommand

Due to some limitations in the Robot Builder Java code, declarations are not supported so I cannot add anything substantial to the creation of these commands. They are still useful in that they are just as capable as any other command. I will send some changes to collabnet to see if we can get the developers of Robot Builder to add the declaration tags for the export yaml file.

### BatteryVoltage

Finished. Please read documentation in RobotBuilder for more info.

### LidarDistance

Finished. Please read documentation in RobotBuilder for more info.

### SocketVision

Finished. Please read documentation in RobotBuilder for more info.
