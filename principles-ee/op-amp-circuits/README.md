# Operational-Amplifier Circuits

## Overview

Designed and tested **LM741 inverting and non-inverting amplifier circuits** to study closed-loop gain, saturation, feedback, output loading, and the difference between an ideal op-amp model and real hardware.

## Laboratory Setup

The experiments used a Keithley 2231-30-3 power supply, Keysight 34461A digital multimeter, breadboard, resistors, a variable 10 kΩ resistor, and 741 op-amps.

Voltage-divider networks were included at the amplifier inputs to reduce the applied signal and help keep the op-amp inside its linear operating region rather than driving directly into saturation.

## Inverting Amplifier

The inverting configuration uses negative feedback, with ideal closed-loop gain determined primarily by the resistor ratio:

    K = -Rf / Rs

The negative sign represents the 180-degree inversion between input and output. The experiment examined the useful linear region as well as the point where the requested output could no longer be produced because of the supply rails.

## Non-Inverting Amplifier

The non-inverting configuration was also built and measured. Its ideal closed-loop gain follows:

    K = 1 + Rf / Rs

This configuration preserves input polarity while providing amplification through negative feedback.

## Output Loading

To investigate non-ideal output behavior, load resistors were connected to the amplifier output while the source remained fixed. Recorded load tests included approximately:

| Load Resistance | Load Current |
| ---: | ---: |
| 20 kΩ | 0.50 mA |
| 9.8 kΩ | 1.0 mA |
| 5.06 kΩ | 1.97 mA |

As load resistance decreased, the demanded output current increased. This portion of the experiment connected the ideal voltage-gain model to the practical current-driving limitations of a real op-amp.

## Skills Demonstrated

LM741 Op-Amps • Negative Feedback • Inverting Amplifiers • Non-Inverting Amplifiers • Closed-Loop Gain • Saturation • Output Loading • DMM Measurement • Breadboarding

**Context:** Collaborative Principles of Electrical Engineering I laboratory project.
