# Sequential Logic & Finite-State Machine

## Overview

Designed, simulated, and physically implemented sequential logic using **latches, D flip-flops, and a synchronous finite-state machine**. Unlike combinational logic, the circuit's output depended on stored state as well as present input.

## Design Process

The components were first modeled in **Vivado** and verified using simulation testbenches. For the state machine, excitation equations and a state-transition table were derived before the hardware implementation.

The physical FSM used:

- D flip-flops for state storage
- 74LS08 AND gates
- 74LS32 OR gates
- LEDs for Q1, Q2, and output Z
- A manually controlled clock generator

Both flip-flops shared the same clock so state variables updated together on each rising edge.

## State Logic

The first D input was generated from feedback involving Q1' and Q2. The second D input used an OR relationship involving input X and Q2'. The output Z was generated from Q2' and Q1.

A mechanical-switch clock circuit using asynchronous flip-flop inputs provided clean observable state transitions. LEDs made it possible to monitor Q1, Q2, and Z while stepping through the machine.

## Engineering Workflow

This lab connected the full sequential-design workflow:

    Behavioral requirement
          ↓
    State / excitation equations
          ↓
    Vivado implementation
          ↓
    Testbench simulation
          ↓
    74LS hardware implementation
          ↓
    LED-based verification

## Skills Demonstrated

Sequential Logic • Finite-State Machines • D Flip-Flops • State Tables • Excitation Equations • Vivado • Verilog • Testbenches • Hardware Verification

**Context:** Collaborative Digital Logic Design laboratory project.
