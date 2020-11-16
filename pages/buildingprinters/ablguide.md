# How to Setup Auto Bed Leveling

This is a guide to auto bed leveling. It does not explain the various options of bed leveling sensors as there are continuously new products and models/iterations released. Research for the best option for your use-case is highly recommended.

## Prerequisites

- Access and knowledge to modify and flash the firmware
- Paper or sticky note for manual bed calibration
- Tools and parts to mount the probe/sensor
- Somewhat level print bed and relatively clean hotend nozzle

## Basic Steps

1. Install the sensor.
2. Modify and flash the firmware.
3. Calibrate the sensor.
4. Set the slicer settings.

## Installing the sensor

Before beginning, it is highly recommended that the printer is unplugged and unpowered.

Usually, auto bed leveling sensors are mounted on the printhead. Some printers may have the option to mount it stock while some require some form of adapter. A 3D-printed adapter and with some small machine hardware like screws and nuts are usually adequate.

When mounting, make sure when the probe activate, the nozzle still has a small gap before touching the bed.

After the sensor is physically mounted, its cable needs to be plugged into an appropriate plug in the controller board. Some stock printers may require some additional components so check with the menu. For printers such as ones with an upgraded or modified board that have the appropriate connectors for the sensor, refer to the specific menu. Note that the sensor may come with a different connector compared to the one of the board. In this case, you may have to make some small modifications like modifying the connector, which is possible but may not be recommended, or replacing with another connector. Make absolutely certain that the connectors are correctly installed as mistakes can cause part damage and/or a short out.

## Firmware Setup

Check with the specific firmware used on the 3D printer. Different firmware, sensor and board combinations may yield different settings. But in general, there are usually a number of settings, such as the probe offset, probing speed and mesh leveling method, that needs to be set.

After the firmware configuration is setup, flash the firmware onto the printer and turn it on.

## Sensor Calibration

With the printer turned on, make sure the sensor works and activates by triggering it with something else like your hand if possible first before testing on the print bed. Be always ready to stop the printer in the case of a malfunction.

After confirming that the sensor works, home the print bed. With probe homing, it may some millimeters back up afterwards so make sure the Z height is at 0. Manually use the motor controls to adjust the Z height while measuring for the correct nozzle distance. Then, assuming the probe offset is 0, set and save the offset to the Z height which has the correct distance from print bed. Auto home again. Check if the new offset is correct and fine-tune if necessary.

Finally, test the auto bed leveling with G29 and make sure it probes within the area of the bed and measures as much of the bed area as possible.

## Setting the Slicer

It is usually necessary to at least add the G29 command for auto bed leveling to the start code. You may also want to set a certain probe setting such as the mesh type depending on the print surface being used.
