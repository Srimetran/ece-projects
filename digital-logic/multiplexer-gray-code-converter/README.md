# Multiplexer-Based Binary ↔ Gray Code Converter

## Overview

Designed and built a **3-bit binary-to-Gray encoder and Gray-to-binary decoder** using 74LS-series MSI components. The project used **74LS151A 8-to-1 multiplexers** for encoding and **74LS86A XOR gates** for decoding.

## Binary → Gray Encoder

Three switches represented the binary input bits and were connected to the multiplexer select inputs. The multiplexer data inputs were programmed with the required Gray-code truth-table patterns:

- G2 multiplexer inputs: 00001111
- G1 multiplexer inputs: 00111100
- G0 multiplexer inputs: 01100110

Each multiplexer output drove an LED, allowing every 3-bit binary input combination to be checked visually.

## Gray → Binary Decoder

The Gray outputs were fed into XOR logic using:

    B2 = G2
    B1 = G2 XOR G1
    B0 = G2 XOR G1 XOR G0

Three additional LEDs displayed the reconstructed binary value.

## Verification

All eight possible 3-bit input combinations were tested. The encoder produced the expected Gray code and the decoder successfully reconstructed the original binary value for the tested combinations.

## Skills Demonstrated

Multiplexers • XOR Gates • Gray Code • Binary Encoding/Decoding • Truth Tables • 74LS151A • 74LS86A • Verilog • Breadboarding

**Context:** Collaborative Digital Logic Design laboratory project.
