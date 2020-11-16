# Motion System

*Note: This guide will only focus on the Cartesian motion system and its various kinematics.*

The motion system consist of the components that make up the linear motion mechanism, such as stepper motors, lead screws, timing belts, etc. There are various types of 3D printers but the Cartesian is the most popular and overall requires the least calculation for print moves by the controller board. Within Cartesian printers however, there are also different kinematics such as the Mendel/i3-style, H-Bot, CoreXY, each with their strengths and weaknesses. Learn more about the strengths and weaknesses of these Cartesian kinematics [below](#comparison-of-various-cartesian-kinematics).

## Components

### Belts

Belts are mostly used for translating the rotational force of the X and Y motors into linear motion for the X and Y axes. However, they require tensioning to maintain accuracy. Some are stiffer than others and thus require less tensioning and are well-suited for Cartesian motion systems with a long belt system such as CoreXY. They are normally preferred for lead screws for X and Y movement as they easily move much faster than the alternative.

Currently, GT2 belts, which are designed specifically for linear motion, are the standard for most 3D printers and is likely what nearly everyone will use. They are designed to account for backlash, essentially the play either in a threaded rod or a belt/pulley when the direction changes.

### Lead Screws

Also known as threaded rods, lead screws are usually used only on a Cartesian printer's Z axis in most cases, as it is strong and fast enough for its use case. Compared to belts, lead screws are much stiffer and only need periodic lubrication, usually with synthetic grease. Note that, because lead screws are relatively difficult to machine and can hence be somewhat untrue, it is usually best to avoid over-constraining lead screws by not fixing it at multiple points. Also, most threaded rod standards, with a few exceptions, have high backlash but it is not that important as the Z axis mostly moves in one direction during prints.

## Comparison of Linear Motion Systems

In 3D printers, there are three main types of linear motion systems used: V-rollers, hardened rods and bearings and linear rails.

### V-rollers

These are usually plastic wheels which ride on aluminum extrusion. Very common on budget printers, they are the most affordable option but may not be ideal for faster or higher-temperature printing.

Pro's

- Very affordable
- Works for most use cases

Con's

- Excessive wear (e.g. grooves) if tightened properly
- May require tightening once in a while
- Tends

### Linear Rod and Bearings

The linear rod, usually made of aluminum, are reasonably straight, round and solid. The bearing, which can be made of a multitude of materials, essentially slides around the rod. There needs to be at least two linear rods and bearings in order to constrain to linear motion as the rods are round and the bearings can hence rotate around its longitudinal axis. Also, alignment, especially for ones with bad tolerances, can be especially difficult as any slight deviations in the linear rod or if the rods or bearings are not parallel cause the load to be stuck or seize in place. Misalignment can cause excessive wear and sometimes "flat spots" and so should be immediately rectified.

<!-- TODO: Compare different types of linear bearings -->

Pro's

- Last for a long time with proper setup and maintenance
- Usually has better tolerances than V-rollers

Con's

- Easily misaligned which causes excessive wear
- Sometimes, the rod and bearing needs to be matched (e.g. from the same manufacturer and produce line-up) for proper tolerances

### Linear Rails

A linear rail is a rail with a carriage that slides. Usually, recirculating ball bearings in the carriage contact the rail.

Pro's

- Usually significantly stiffer than linear rods
- Isolates strictly linear motion, unlike linear rods
- Usually manufactured with much tighter tolerances
- No need of alignment

Con's

- Expensive
- Ball bearings fall off if the carriage falls off

## Comparison of Various Cartesian Kinematics

### Mendel/i3-style

Mendel/i3-style printers have independent X, Y and Z axes where each motor moves on axis, an XZ gantry moves the printhead in the X and Z axes and the print beds moves in the Y axis.

Pro's

- Frame is affordable to manufacture
- The most simple kinematics

Con's

- Not space efficient (bed takes up twice the space of itself)
- Heavy bed on the Y axis; poor print quality on Y axis
- Motors move independently of each other

### CoreXY

CoreXY printers have an independent Z axis and an XY gantry where the X and Y motors each move the X and Y axis together at the same time.

Pro's

- Fast XY print movements as X and Y motors work together
- Virtually no difference in print quality between the X and Y faces of prints
- Space efficient

Con's

- Requires a rigid cube frame and pulley system (usually)
- Very long belts requires stiffer belts and more belt tensioning
- Misaligned belts or pulleys can result in major print issues

### H-Bot

Work in progress!

<!-- H-Bot printers have similar kinematics to CoreXY but uses a different belt drive system.

Pro's

- Fast XY print movements as X and Y motors work together

Con's

- Requires a rigid cube frame and pulley system (usually)
- Misaligned belts or pulleys can result in major print issues -->
