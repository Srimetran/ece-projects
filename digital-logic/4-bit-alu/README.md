# 4-Bit Arithmetic Logic Unit (ALU)

## Overview

Designed and implemented a 4-bit arithmetic unit capable of performing four operations selected by a two-bit control input:

- Addition
- Subtraction
- Increment
- Decrement

## Architecture

The design combines multiplexers with a 4-bit binary adder. The multiplexer controls the operand supplied to the adder, while XOR-based carry-in generation supports the required arithmetic behavior.

Subtraction and decrement operations use two's-complement arithmetic. The project also examined signed 4-bit overflow: values outside the representable range of -8 to +7 demonstrate the limitations of fixed-width arithmetic.

## Key Takeaways

- 4-bit arithmetic datapath design
- Multiplexer-based operation selection
- Binary addition and subtraction
- Two's-complement representation
- Carry-in/carry-out behavior
- Signed overflow and fixed-width arithmetic
- Hardware implementation and verification

**Context:** Collaborative Digital Logic Design laboratory project.
