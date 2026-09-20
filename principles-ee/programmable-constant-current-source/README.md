# Programmable Constant-Current Source

## Overview

Designed a mixed hardware/software system intended to regulate load current from a programmable setpoint. The project combined an **Arduino, 4-bit R-2R DAC, op-amp circuitry, current-sense resistor, ADC measurement, and closed-loop control code**.

## System Architecture

    Target Current
          ↓
    Arduino Controller
          ↓
      4-bit DAC Code
          ↓
       R-2R Ladder
          ↓
    Analog Control Voltage
          ↓
     Op-Amp / Load
          ↓
      Sense Resistor
          ↓
    Amplified Sense Voltage
          ↓
      Arduino ADC
          ↓
       Feedback

The documented code used four digital pins for the DAC and assumed a **5 V ADC reference**, **10-bit ADC (0–1023)**, **15 Ω sense resistor**, and **sense gain of 11**.

## Current Measurement

The Arduino read the amplified sense voltage from analog input A0, converted the ADC reading back into voltage, divided by the amplifier gain to estimate the voltage across the sense resistor, and calculated current from:

    I = Vsense / Rsense

The result was converted to milliamps and compared against the requested current.

## Feedback Logic

The controller compared measured current against the target. If the current was too low, the 4-bit DAC code was incremented; if it was too high, the DAC code was decremented. With four bits, the controller had **16 DAC codes (0–15)**, so adjustment occurred in discrete steps.

## Validation & Debugging

The **hardware was constructed successfully**, and the DAC value changed when the setpoint or load was changed. However, the final measured current did **not reliably track the requested setpoint**. The team repeatedly debugged the Arduino code with assistance during the lab, but the software/control issue remained unresolved.

That limitation is intentionally documented rather than presenting the prototype as fully functional. The debugging process still demonstrated an important engineering reality: individual subsystems can appear correct while the integrated closed-loop system fails to meet its requirement.

The report also considered a rapidly varying load. At around **100 Hz**, the Arduino/DAC update rate or op-amp control-loop response could cause the current regulation to lag changes in load resistance.

## Skills Demonstrated

Mixed-Signal Design • R-2R DAC • Operational Amplifiers • Current Sensing • Arduino GPIO/ADC • Bitwise Operations • Feedback Control • Embedded Debugging • System Integration

**Context:** Principles of Electrical Engineering I laboratory project.
