# Resistive Networks & Voltage Division

## Overview

Designed, built, and measured resistor networks to connect circuit-analysis theory with real hardware. The lab focused on equivalent resistance, proportionality, voltage division, resistor tolerance, and power constraints.

## Equivalent Resistance & Proportionality

The measured input current at 10 V was **1.664 mA**, very close to the predicted **1.67 mA** and within the expected tolerance range. From the measured current, the equivalent resistance was approximately **6009 Ω**, inside the predicted **5.7 kΩ–6.3 kΩ** range.

The measured proportionality coefficient was approximately **0.254**, compared with a predicted range of **0.2375–0.2625**.

## Voltage-Divider Design

A second circuit was designed to satisfy:

    Vout ≈ 0.75 Vin

while keeping source power below **0.3 mW**. The measured divider coefficient averaged approximately **0.75**, and measured source power was about **0.2468 mW**, satisfying the design objective.

The voltage sweep from 10 V down to 2 V showed the output decreasing approximately proportionally with the input, reinforcing the linear behavior of a purely resistive network.

## Why This Matters

This project was not just about calculating resistor combinations. It required translating a specification into a physical circuit, accounting for component tolerance, checking the power budget, and determining whether measured results were close enough to theory to validate the design.

## Skills Demonstrated

Series/Parallel Networks • Equivalent Resistance • Voltage Division • Resistor Tolerance • Power Analysis • Breadboarding • DMM Measurement • Theory-vs-Measurement Validation

**Context:** Collaborative Principles of Electrical Engineering I laboratory work.
