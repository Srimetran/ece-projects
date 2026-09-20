# Programmable Constant-Current Source

## Overview

Developed an Arduino-controlled constant-current source combining digital control with analog circuitry. The system used a 4-bit R-2R DAC, operational-amplifier stages, a current-sense resistor, and Arduino control logic.

## System Architecture

The Arduino drives four digital lines representing a DAC code from 0 to 15. An R-2R ladder converts that code into an analog control voltage. Op-amp circuitry uses the control signal as part of the current-source implementation, while a sense resistor provides a measurable voltage related to load current.

The documented controller uses a 10-bit Arduino ADC reference, a 15-ohm sense resistor, an op-amp sense gain, a maximum target current of 10 mA, and 0.5 mA setpoint resolution.

## Software Control

The Arduino code includes a helper routine that writes individual bits of the DAC code to four digital output pins. The project therefore combines embedded software with an analog feedback/control circuit rather than treating the hardware and software as separate systems.

## Engineering Concepts

- Constant-current source design
- R-2R digital-to-analog conversion
- Operational amplifiers
- Current sensing
- Analog feedback/control
- Arduino GPIO and ADC concepts
- Bitwise operations
- Embedded hardware/software integration

**Context:** Principles of Electrical Engineering I laboratory project.
