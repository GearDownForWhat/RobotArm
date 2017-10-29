# RobotArm
4 Axis Stepper Non-cartesian Robot Arm

I run this on an arduino DUE with a CNC sheild and DRV8825 stepper drivers.


If you would like to use serial commands, make sure you have the serial monitor set to "newline"
You can test the movement of each joint by opening up the serial monitor and typing:

M5 J0 P10          <-This will position the base 10 degrees clockwise
"M5" is a command to move joints manually, the "J0" chooses the joint to move, and "P10" means position at 10 degrees.

You can also send XYZ Coordinates through serial, for example
G00 X250 Y10 Z40           <-use this to move directly to the coordinate
or
G01 X210 Y10 Z40          <-use this to move in a straight line
