# ftc_pixy
Pixy interface code for FTC Java SDK

This code provides an interface to the Pixy camera (http://charmedlabs.com/default/pixy-cmucam5/) for use with FIRST Tech Challenge Java code. It is set up to be a named I2C device type selectable in the robot configuration menu. It is designed to work with the modified firmware provided by Andrew De Vries (see this thread https://ftcforum.usfirst.org/forum/ftc-technology/59240-ftc-mr-core-device-interface-module-charmedlabs-pixy-cmu5). It started out based on code from Lee Acton which was posted in this thread https://ftcforum.usfirst.org/forum/ftc-technology/android-studio/7211-i2c/page2 and using the Lego I2C protocol for the Pixy.

The modified firmware can be downloaded from here: https://github.com/Andrewiski/ControlFreaks_ftc_app/blob/master/pixy/pixy_firmware.hex

The current code is designed to work with the modified firmware and use the FTC I2C protocol.

We use the Pixy connected to a REV Robotics Expansion Hub using a level shifter. We took a 10 pin ribbon cable and cut it in half and then soldered jumper wires to the four pins needed for I2C (from the 10 pin ribbon cable, pins 2, 5, 6, and 9).

Currently, the code does not work for finding color codes (a combination of up to five color signatures). The code could be easily modified to support those modes, if desired.
