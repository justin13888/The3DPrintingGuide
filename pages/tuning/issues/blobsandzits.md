# Blobs and Zits

During a 3D print, the extruder constantly changes speed or stops and starts. While it may normally produce uniform extrusions, sometimes, there may be surface blemishes due external variables known as blobs and zits. For example, when at printhead prints an outer shell and returns to the start position, it may leave a mark. However, using your preferred slicer, there are usually ways to minimize the appearance of the blemish.

## Retraction and coasting settings

When observing the perimeter of a part being printed, see if the blemish appears when the extruders starts printing, later after the perimeter is printing or after the extruder comes to a stop.

If the issue appears immediately after starting the perimeter, **adjust the retraction distance** as it is likely priming too much filament.

If the issues occurs after the end of the perimeter when the extruder stops, **increase the coast distance** until it disappears. Usually, a few 1/10th of a millimeter adjustment is adequate.

## Avoiding unnecessary retractions

While the retraction and coast settings may help avoid this defect, it is possible that avoiding retractions completely is better. Particularly for Bowden extruders, retractions may cause other issues. So try **only retract when crossing open spaces** or outside of prints where stringing for example is visible.

## Turn on Wipe Nozzle

To avoid creating a blob when the extruder stops after printing a perimeter, you can **turn on the "Wipe Nozzle" option** in your slicer and start from around 5 mm of wipe distance. You can also turn on retraction during the wipe.

## Change the start point location

If you cannot resolve this issue, you can select a less visible start location for printing the perimeter. Some slicers also allow the option to randomize the start point.
