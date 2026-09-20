# R-2R Digital-to-Analog Converter

## Overview

Built and analyzed a **4-bit resistor-ladder DAC** driven by Arduino digital I/O. The project connected binary values to analog output voltage and then investigated how output loading and buffering affect a real DAC.

## DAC Relationship

The 4-bit ladder produces a weighted analog output based on the four digital input voltages. The report expresses the loaded output relationship as:

    Vload = Vbit3/2 + Vbit2/4 + Vbit1/8 + Vbit0/16

The measured DAC voltages closely matched the expected values from the theoretical analysis.

## Output Loading

The DAC was also modeled using its **Thevenin equivalent**. This made it possible to reason about how load resistance changes the delivered voltage and power instead of treating the DAC as an ideal voltage source.

From the reported values:

    Vth ≈ 4.69 V
    Rth ≈ 10 kΩ
    Isc = Vth / Rth ≈ 0.47 mA

The short-circuit current represents the maximum unbuffered output-current condition in the Thevenin model.

## Arduino Drive Limits

The lab also considered the source-side limit of the Arduino outputs. Using the lab's stated **40 mA per digital I/O at 5 V**, the calculated per-pin power was 0.2 W and the four-I/O total was 0.8 W for the theoretical exercise.

## Why Buffering Matters

An op-amp buffer can isolate the resistor ladder from the load. The ladder then establishes the desired voltage while the buffer supplies load current, reducing the effect of load resistance on DAC accuracy.

## Skills Demonstrated

R-2R Ladders • DACs • Binary Weighting • Arduino GPIO • Thevenin Equivalents • Loading Effects • Op-Amp Buffering • Mixed-Signal Measurement

**Context:** Principles of Electrical Engineering I laboratory project.
