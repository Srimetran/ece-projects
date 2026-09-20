# Combinational Logic & Hazard Analysis

## Overview

Minimized and implemented combinational logic while exploring two practical digital-design ideas: implementing logic entirely with **NAND gates** and identifying/removing **timing hazards**.

## NAND-Only Implementation

The original AND, OR, and NOT operations were transformed into NAND-based equivalents. Because NAND is a universal gate, the same Boolean function can be implemented without requiring separate gate families.

This exercise connected Boolean identities to physical implementation: an algebraically equivalent expression can have a very different gate-level structure.

## Karnaugh-Map Minimization

Karnaugh maps were used to simplify the target functions and identify groupings that reduce the required logic. The minimized expressions were then translated into gate-level circuits.

## Hazard Analysis

The project also examined how different propagation delays through separate logic paths can produce a short unwanted output transition—a **glitch or hazard**—even when the steady-state Boolean values are correct.

K-map analysis was used to identify the missing redundant grouping needed to maintain a stable output during an input transition. The corrected implementation was then used to avoid the glitch.

## Skills Demonstrated

Karnaugh Maps • NAND-Only Logic • Boolean Minimization • Combinational Circuits • Static Hazard Analysis • Propagation Delay • Breadboard Debugging

**Context:** Collaborative Digital Logic Design laboratory project.
