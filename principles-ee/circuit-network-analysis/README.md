# Circuit Network Analysis: Superposition, Thevenin & Norton

## Overview

Applied **superposition, Thevenin equivalence, and Norton equivalence** to resistor networks and compared analytical predictions with physical measurements.

## Superposition Experiment

For the resistor network used in the lab, nodal analysis produced:

    Vout = (Vs1 + Vs2) / 3

The circuit was tested with multiple source combinations:

| Vs1 | Vs2 | Calculated Vout | Measured Vout |
| ---: | ---: | ---: | ---: |
| 8 V | 10 V | 6.00 V | 6.00 V |
| 6 V | 12 V | 6.00 V | 6.00 V |
| 12 V | 8 V | 6.67 V | 6.67 V |

With each source considered independently, the chosen 10 kΩ network reduced to:

    Vout1 = Vs1 / 3
    Vout2 = Vs2 / 3

The measured proportionality coefficients were close to the theoretical **1/3** value: the report gives average values of **K1 ≈ 0.3322** and **K2 ≈ 0.35**.

## Thevenin / Norton Analysis

The second portion treated a larger resistor network as a two-terminal source network. A Thevenin equivalent replaces the original network with **Vth in series with Rth**; the corresponding Norton model uses **In in parallel with Rn**. The lab used a 12 V source and a designed divider/load network to compare the simplified equivalent behavior with the original circuit.

## Skills Demonstrated

Nodal Analysis • Superposition • Thevenin Equivalents • Norton Equivalents • Linear Circuit Analysis • Breadboarding • Experimental Verification

**Context:** Collaborative Principles of Electrical Engineering I laboratory project.
