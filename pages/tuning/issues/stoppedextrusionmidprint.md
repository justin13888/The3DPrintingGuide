# Stopped Extrusion Mid-Print

There are only a common causes when a printer extrudes properly at the beginning of the print but suddenly stops extruding afterwards.

## The filament ran out

**Check if the filament ran out**. If the printer has a filament run-out sensor, it will likely have paused so you can reload new filament and resume the print. Otherwise, you will have to reload new filament and restart instead.

## The filament is stripping against the drive gear

In the extruder, the drive gear pushes the filament through a nozzle. However, when the extruder and/or hotend fails to keep up with the extrusion speed, it the drive gear may strip the filament until there is no more material to hold on to. **Refer to the [Grinding Filament](grindingfilament.md) article** to learn more.

## The extruder is clogged

It is possible that the extruder may be clogged with dust, debris, loose filament, etc. such that it becomes clogged. There are other possible causes thus also **refer to the [No Extrusion at the Start of Print](noextrusionatstart.md) article** for more details.

## The extruder stepper driver is overheating

With insufficient cooling, the extruder stepper driver may overheat. Because these drivers typically have a thermal cut-off, it will stop the driver from working if the temperature is too hot. To resolve this issue, **turn off the printer and allow the electronics to cool down**. In the future, you can also add additional cooling to the electronics.
