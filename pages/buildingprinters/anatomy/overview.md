# 3D Printer Anatomy

This is a list of most 3D Printer components with its basic function(s).

![Illustrated Diagaram of the 3D Printer Anatomy (Source: MatterHackers)](https://lh3.googleusercontent.com/vy2gmNQu0ZCXauAxKtD2J1Q6jinZmBU9fxo-nE17DEJdg-vVKAOPm-tqx42aaXFn5G8y2h4jdkqGXZKDovjJUfh1Pzs)

## [Frame](frame.md)

The Frame is a structural component of 3D Printers and must withstand the mechanical loads that the motion system generates. It is the foundation of a 3D printer and largely determines its size and structural rigidity. Most printers today use aluminum (or aluminium) extrusions although early printers used materials such as lasercut plywood.

## [Print Bed](bed.md)

The print bed is the surface which the object is printed on. There are various materials such as glass or aluminium and can be heated which help adhesion for many filament materials.

Most print beds are heated in order to prevent warping due to thermal contraction.

## [Bed Surface](bedsurface.md)

The bed surface help with bed adhesion and can be removed easily after prints. Bed surfaces come with many different materials so for best results, invest in a build surface best suited for the print material.

## [Bed Leveling](bedleveling.md)

Bed leveling, as the term suggests, compensates for level build surfaces to ensure the optimal bed adhesion and base surface quality.

## [Extruder](extruder.md)

There are two main categories of extruders: Direct-drive (DD) and Bowden. Some are geared down to allow for a weaker motor and some are dual-drive to improve filament grip.

![Illustrated diagram of the extruder (Source: MatterHackers)](https://lh3.googleusercontent.com/76t-Q-wj6qCWPOeIJXgB46fNZTGKU9IS8LXmu7PbQuA46x8-y93xbOAACS2vUgTeU66FlCmKKC3wlRMBOYMUV9Gx_A)

## [Hot End](hotend.md)

The hot end is responsible for heating and extruding the filament. All metal hot ends are able to reach much higher temperatures and print a wider range of materials. On the contrary, PTFE or PEEK lined hot ends are usually more affordable but can only print at a lower temperature and a smaller range of materials.

### Heater Cartridge

As the name suggests, the heater cartridge heats up the hotend and in turn the filament.

### Thermistor, Thermocouple and RTD

Thermistors, thermocouples and RTDs are all common types of sensors that measure temperature.

<!-- TODO: Explain benefits and weaknesses of each type -->

### Nozzle

The nozzle is threaded at the end of the hotend where the melted filament is extruded. They are interchangeable and come in varioius materials and sizes. 0.4 mm is the most common and all-purpose size that most printers come default with.

### Part Cooling Fan

This fan immediately cools down the extruded plastic which help certain filaments hold its shape.

## [Motion System](motionsystem.md)

The Motion system consist of the components that make up the linear motion mechanism, such as stepper motors, lead screws, timing belts, etc. There are various types of Cartesian motion systems such as the Mendel-style, H-Bot, CoreXY, each with their strengths and weaknesses.

<!-- TODO: Compare benefits of each -->

### End Stops

These are small, usually inexpensive switches that are closed when an axis moves to the end. They are most commonly used during homing.

### Leadscrews or Threaded Rods

These are usually used on a cartesian printer's Z axis although other axes can use it as well. Leadscrews are usually very difficult to machine and is somewhat untrue. Therefore, it is usually best to avoid over-constraining leadscrews such as adding a fixed bearing around multiple ends of a leadscrew.

### Belts

Belts are usually used for translating the rotational force of the X and Y motors into linear motion for the X and Y axes. They require tensioning and not all are made equally. Some are stiffer than others and thus require less tensioning and are well-suited for Cartesian motion systems with a long belt system such as CoreXY.

### Stepper Motors

Stepper motors rotate in specific increments, allowing precise control over their position. Most printers today use NEMA 17.

## [Electrical Components](electrical.md)

### Power Supply

This converts the grid electricity from the wall into low voltage DC power that can be consumed by the printer. Although 3D printer traditionally run on 12 volt systems, today, 24 volts is becoming much more popular.

### Controller Board

This is the brain's of the printer that parses and executes the commands in G-Code.

#### Stepper Drivers

These chips control the stepper motors through the voltage and current. Most motherboards have these stepper drivers built-in while some are interchangeable so it can be replaced or upgraded.

### Screens and Other User Interfaces

Some printers have a screen that can directly control the printer. Some are basic black and white displays while others are multi-coloured touchscreens.

## Further Reading

- [Frame](frame.md)
- [Print Bed](bed.md)
- [Bed Surface](bedsurface.md)
- [Bed Leveling](bedleveling.md)
- [Extruder](extruder.md)
- [Hot End](hotend.md)
- [Motion System](motionsystem.md)
- [Electrical Components](electrical.md)
