# FSM Traffic Signal Controller

## Overview

Designed a demand-driven digital traffic-signal controller for a main road and cross road. Under normal conditions, the main road remains green. A pedestrian walk request initiates a timed sequence that transitions the intersection through amber, red, cross-road green, and cross-road amber before returning to the default state.

## Architecture

The controller was designed as a finite-state machine with:

- State storage using flip-flops
- Combinational transition logic
- Output logic for the traffic signals
- A clock generated with a 555 timer in astable mode
- A pedestrian request input

A state diagram was used to define the controller behavior before deriving excitation logic and constructing the hardware schematic.

## Testing & Debugging

The implementation exposed an active-low output behavior that initially made the lights appear inverted. Debugging traced the behavior to the output convention rather than the state-transition logic. A logic probe was also part of the hardware-debugging process.

## Key Takeaways

- Finite-state-machine architecture
- State diagrams and excitation equations
- Sequential and combinational logic integration
- 555 timer clock generation
- Active-high vs. active-low logic
- Hardware debugging and verification
- Translating a behavioral specification into a digital controller

**Context:** Collaborative Digital Logic Design laboratory project.
