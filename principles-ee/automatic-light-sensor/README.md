# Automatic Light Sensor

## Overview

Built an automatic lighting circuit that converts ambient light level into an electrical decision using a **photoresistor (LDR), resistor network, operational amplifier, and LED**. The goal was to make the LED turn on in darkness and turn off under brighter conditions.

## Circuit Behavior

The photoresistor changes resistance with incident light. That changing resistance changes the voltage applied to the op-amp's non-inverting input. The other input was held at a **7.5 V reference**, allowing the op-amp to act as a comparator.

### Dark condition

When the environment became dark, the photoresistor resistance increased. This raised the non-inverting input above the 7.5 V reference. The op-amp output switched toward **+15 V**, driving current through a **1 kΩ resistor and the LED**, which turned the light on.

### Bright condition

Under brighter light, the LDR resistance decreased. The non-inverting input dropped below the reference voltage, causing the op-amp output to swing negative and cutting off LED current.

## Signal Flow

    Ambient Light
         ↓
    Photoresistor
         ↓
    Voltage Signal
         ↓
    Op-Amp Comparison
         ↓
    LED ON / OFF

Instead of using software to decide whether the light should turn on, the behavior is produced directly by analog circuitry.

## Skills Demonstrated

Photoresistors • Sensor Interfacing • Voltage Dividers • Op-Amp Comparators • Threshold Detection • LED Current Limiting • Breadboarding • Analog Control

**Context:** Principles of Electrical Engineering I laboratory project.
