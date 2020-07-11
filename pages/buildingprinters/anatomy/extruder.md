# Extruder

The ultimate purpose of the extruder is to control the filament travel. In other words, it extrudes and retracts filament. But there are two main categories of extruders: Direct-drive (DD) and Bowden. Some are geared down to allow for a weaker motor and some are dual-drive to improve filament grip.

<!-- TODO: Explain more about dual-drive and gearing ratios -->

## Direct-Drive Extruders

Direct-drive extruders are mounted on the printhead feed filament through a much shorter path, either with or without a very short, straight PTFE tube.

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

- **Ligher Printhead**: The printhead loses the weight of the extruder and/or motor, allowing faster print with less print artifacts.
- **Larger Build Volume**: A more compact printhead allows for a higher build volume.

Con's:

- **More Powerful Motor**: Due to the added friction from the Bowden tube, it requires a more powerful motor.
- **Less Precise Extrusions**: The Bowden tube does not perfectly constrain the filament path, allowing the filament to extend within the tube.
- **Slower Retractions**: Due to the less contrained Bowden tube, longer retractions are usually needed to avoid stringing.
- **Smaller Range of Materials**: Some flexible or abrasive materials easily bind or wear the Bowden tube.
