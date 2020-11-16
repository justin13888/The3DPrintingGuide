# Electrical Components

## Components

### Power Supply

The power supply converts the grid electricity from the wall into low voltage DC power that can be consumed by the printer. Although 3D printer traditionally ran on 12 volt systems, today, 24 volt systems have become the norm.

### Stepper Motors

Stepper motors rotate in specific increments (e.g. 1.8°/step), allowing precise control over their position. Most 3D printers today use NEMA 17 motors.

### Controller Board

This is the brain's of the printer that parses and executes the commands in G-Code. In the past, many printers ran on Arduino boards with add-on boards called a "shield". Today however, it is much more common to find printers with dedicated microcontroller boards. Although 8-bit boards have been the standard for some time, increasingly common and faster 32-bit boards offer stronger processing speeds and allow for more advanced firmware features.

### Stepper Drivers

These chips control the stepper motors by regulating the voltage and current. Most motherboards have these stepper drivers built-in or integrated into the board while some are interchangeable as breakout boards so it can be replaced or upgraded.

Although stepper drivers can support either AC or DC current, normally for 3D printers, they strictly use DC current from the controller board or some form off extension board. There are also various current output ratings which restricts the power allowed to the stepper motor. Many drivers today also support microstepping which divides every step of the motor into even smaller steps by sending precisely enough current to hold the motor in between steps. 1/16th micro-stepping is pretty common while some are capable of even 1/256th microstepping.

### Screens and Other User Interfaces

Some printers have a screen that can directly control the printer. Some are basic black and white displays while others are multi-coloured touchscreens.

## Temperature Sensors

There are mainly three types of temperature sensors used in 3D printers: thermistors, PT100 sensors and thermocouples.

### Thermistors

Thermistors work with most 3D printer controller boards. They usually work up to 300°C although there are some "high-temperature" thermistors which can work upwards of 450°C. In rare cases, in high-temperature printing (300°C+), one low-temperature and one high-temperature thermistor can be used together to measure the extruder temperature in the whole temperature range and ensure accuracy.

### PT100 Sensors

PT100 sensors, the most popular type of RTD are usually preferable for serious, high-temperature and high-performance printing as they are more accurate than thermistors and capable of sensing even higher temperatures. However, most controller boards require a separate amplifier board for it to understand the PT100 sensor.

### Thermocouples

Thermocouples can be used but are generally not preferred. For high-performance or high-temperature printing, a PT100 sensor is usually the better option. However, Type K thermocouples, for example, are still capable of measuring temperatures higher than any 3D printer extruder can produce.

## End Stops

An end stop is a simple circuit board with a switch. It allows calibration of print limits during start up and detection when a printer axis has reached a limit in a certain direction, particularly useful for homing. Usually, there are end stops for minimum and maximum limits of each axis. However, there could be only end stops for the minimum limits with software end stop for the maximum limits. Printers with bed leveling probes do not need Z min end stops and some Trinamic stepper drivers have sensorless homing, which do not require end stops.
