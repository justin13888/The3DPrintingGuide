# Extruder

*This article discusses about the general function of an extruder system and more in-depth on the "cold end" of it or commonly referred as just the extruder. Learn about the "hot end" [here](hotend.md).*

The purpose of the extruder is to extrude filament. The extruder is separated into the "cold end" and the "hot end" where the "cold end" feeds the filament into "hot end" where filament is heated up.

There are two main categories of extruders: Direct-drive (DD) and Bowden. Some are geared down to allow for a weaker motor and some are dual-drive, or more in rare occasions, to improve filament grip. Most geared extruders for desktop printers have a 3-to-1 gearing ratio while some like for industrial printers, feature even higher gearing ratios like 19-to-1.

The "cold end" can either be connected to the "hot end" by a confined PTFE tube and m or a Groove mount where the "hot end" is mounted on the "cold end".

Some extruder systems are also water-cooled, allowing for heated chambers for printing certain engineering filaments that easily warp.

## Direct-Drive Extruders

Direct-drive extruders are mounted on the printhead and feed filament through a much shorter path, either with or without a very short, straight PTFE tube. Most direct-drive extruders have a motor directly connected to it.

However, remote direct-drive extruders have the motor placed stationary off the print head and powered through a flexible shaft. In general, they have the benefits of regular direct drive extruders but also a lighter print head like Bowden setups. However, the flexible shaft must not have any torsional flex under the load of the quick movements of the remote stepper motor.

Pro's:

- **More Precise Extrusions**: Due to shorter and narrower filament path, there are less friction and inaccuracies without a PTFE tube between the filament path.
- **Faster Retractions**: As the extruder is closer to the hotend, faster and shorter retractions are needed for a more confined filament path.
- **Requires a Less Powerful Motor**: Because of the shorter distance between the extruder and nozzle, it requires less torque in the motor.
- **Wider Range of Filaments**: Flexible or abrasive filaments can be more reliably printed from a shorter and more confined filament path.

Con's:

- **Heavy Printhead**: The extruder and usually the motor must be on the printhead, adding additional weight. This results exacerbates printhead wobble and inaccuracy in the X and Y axes. A stiffer linear motion system may be needed to compensate.

## Bowden Extruders

Bowden extruders feed filament from a stepper motor mounted off the printhead through a restricted Bowden tube, normally made from PTFE.

Pro's:

- **Lighter Printhead**: The printhead loses the weight of the extruder and/or motor, allowing faster print with less print artifacts.
- **Larger Build Volume**: A more compact printhead allows for a higher build volume.

Con's:

- **More Powerful Motor**: Due to the added friction from the Bowden tube, it requires a more powerful motor.
- **Less Precise Extrusions**: The Bowden tube does not perfectly constrain the longer filament path, allowing the filament to extend and flex within the tube.
- **Slower Retractions**: Due to the less constrained Bowden tube, longer retractions are usually needed to avoid stringing.
- **Smaller Range of Materials**: Some flexible or abrasive materials easily bind or wear the Bowden tube.
