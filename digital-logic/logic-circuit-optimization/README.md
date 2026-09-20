# Logic Circuit Optimization

## Overview

Analyzed two Boolean functions, built their truth tables, implemented both with physical logic gates, and compared the implementations to determine which realization required less hardware.

## Method

The Boolean functions F(A,B,C) and G(A,B,C) were evaluated for every input combination. AND, OR, and NOT gates were then wired on a breadboard using switches as logic inputs and LEDs/logic probing to observe the outputs.

Testing each truth-table row allowed the physical circuits to be checked directly against the Boolean analysis rather than assuming that correct-looking wiring meant correct operation.

## Result

The measured circuit behavior matched the truth-table outputs. The comparison showed that **function G implemented the same required behavior more efficiently than function F because it used fewer gates**.

The lab also provided practical debugging experience: in at least one test the LED appearance alone was misleading, while the logic probe confirmed that the circuit was wired and operating correctly.

## Engineering Takeaway

Boolean simplification has a direct hardware consequence. Reducing a logical expression can reduce gate count, wiring complexity, propagation paths, and opportunities for implementation errors.

## Skills Demonstrated

Boolean Algebra • Truth Tables • AND/OR/NOT Gates • Logic Optimization • Breadboarding • Logic Probes • Hardware Debugging

**Context:** Collaborative Digital Logic Design laboratory project.
