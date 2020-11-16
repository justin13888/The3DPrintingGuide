# No Extrusion at the Start of Print

There are a few common culprits when no filament is being extruded at start.

<!-- TODO: Edit -->
## The extruder was unprimed

Most extruders have a tendency to ooze plastic while idling at print temperature. If the extruder has lost some plastic before or after prints, it will take a few seconds before plastic starts to extrude again. So make sure to **prime the extruder before the print**. Try using a skirt.

## The nozzle is too close to the bed

If the nozzle is too close to the print bed, there will not be enough room for the plastic to extrude. If the print does not extrude plastic for the first few layers but extrudes normally afterwards, this is likely the issue. Try **adjusting the Z-offset for your auto bed leveling** or **manually leveling the bed**. If you were to slip a single sheet of paper or sticky note, the nozzle should barely tug on the sheet.

## The filament is stripped by the extruder drive gear

The extruder drive gear may be shaving away instead of gripping the filament. If you notice lots of plastic shavings or a part of the filament is missing, the drive gear may have removed too much filament. If that's the case **refer to [Grinding Filament](grindingfilament.md)**.

## The extruder is clogged

The extruder may be clogged if foreign debris or soldified hot plastic is trapped in the nozzle. If that's the case, **refer to [Clogged Extruder](cloggedextruder.md)**.
