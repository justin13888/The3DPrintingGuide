# Tuning Stepper Drivers

This article explains why and how to adjust stepper drivers. It is assumed that the stepper drivers and controller boards are function and connected to a power source (has electricity running).

Keep in mind that there may be some exceptions for the specific model of stepper driver or motor so always refer and check with the information of the stepper driver and the stepper motor from the manufacturers.

## Reasons to Tune the Stepper Drivers

- The motors are running too hot.
- There are layer shifts mid-print or the motors are skipping steps.
- The motors slow down or stop after printing for a while.

## A Note before Beginning

- **DISCLAIMER**: You agree that this guide is meant to be informational and educational and its writers assume **no responsibility** for any personal injuries, damage of property, legal liabilities. Electricity is dangerous. Understand that the following steps have risks that may result in death or serious injuries. **Proceed at your own risk!**
<!-- TODO: Move this disclaimer to a separate page. -->

## Adjusting the VREF

In order to adjust the VREF, first, decide or identify what is the maximum current for the specific stepper motor in Amps and the sense resistor value (Rsense) of the stepper driver in &#8486; (Ohms). This information can usually be found in manufacturer specifications. The motor model can likely be identifiable by looking for a sticker on the body of the motor with a model number. The formula to calculate the VREF is:

VREF = 8 x MAX CURRENT x SENSE RESISTOR VALUE .

**Note:** It is best to have a **safety margin of 10%**.

For example, if the stepper motor has a maximum current of 1.4 A and a sense resistor value of 0.05 &#8486;, the VREF should be 8 x 1.4 x 0.05 = 0.56. With a safety margin of 10%, the VREF is should be 0.56 x 0.9 &approx; 0.5.

To set the VREF, adjust the potentiometer via a small screwdriver (ideally made of ceramic which is non-conductive). Turning clockwise increases the voltage and counter-clockwise decreases. Measure the current VREF with a multimeter for DC voltage. by placing the red probe on the potentiometer and the black probe on a ground pin, either on the driver or alternatively, on the controller board. Keep in mind, a metal or electrically conductive screwdriver can potentially short out the electrical components. Make small screw adjustments followed by a check with the multimeter one at a time to arrive at the targeted VREF.

Alternatively, you can use an alligator clip to connect the positive lead of the multimeter to a metal screwdriver and adjust with the potentiometer while measuring the VREF with the black lead on a ground pin.
