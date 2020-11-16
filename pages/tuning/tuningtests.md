# Tuning Tests

This is a list of common and useful tests used to tune 3D printers.

|                Name                | What is Tests                                  | Fixes                                                                              |
| :--------------------------------: | ---------------------------------------------- | ---------------------------------------------------------------------------------- |
|       Vertical Surface Test        | Ghosting and ringing                           | Lighter printhead, slower acceleration and jerk/junction deviation                 |
|      Horizontal Surface Test       | Perimeter Artifacts                            | Better perimeter slicer settings                                                   |
|     Dimensional Accuracy Test      | Dimensional accuracy                           | [Improving tolerance](improvetolerance.md)                                         |
|           Overhang Test            | Part cooling efficiency                        | Better part cooling, lower print speed                                             |
|           Bridging Test            | Bridging, part cooling efficiency              | better part cooling or slicer settings for bridging                                |
|        Negative Space Test         | Dimensional accuracy, tolerance                | [Improving tolerance](improvetolerance.md)                                         |
|          Retraction Test           | Stringing                                      | Better retraction settings                                                         |
|       Support Material Test        | Support material performance, support settings | Better support slicer settings, using another dedicated support material           |
| Full Bed Dimensional Accuracy Test | Dimensional accuracy across the whole bed      | [Improving tolerance](improvetolerance.md)                                         |
|           Z Wobble Test            | Properly constrained Z axis                    | Remove any constraints in Z lead screw(s) besides motor coupler and lead screw nut |
|          Squareness Test           | Frame squareness on XY axis                    | Square printer frame                                                               |
