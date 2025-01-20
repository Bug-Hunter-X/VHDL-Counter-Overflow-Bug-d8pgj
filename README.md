# VHDL Counter Overflow Bug
This repository demonstrates a common but subtle bug in VHDL code: an integer counter that lacks proper overflow handling.  The `buggy_counter.vhdl` file contains the erroneous code, while `fixed_counter.vhdl` provides a corrected version.

**Problem:** The original counter increments indefinitely, exceeding its defined range (0 to 15). This can lead to unpredictable results or simulation errors.

**Solution:** The corrected counter includes a modulo operation to wrap around when the maximum value is reached, ensuring correct behavior.

This example highlights the importance of carefully considering range limits and potential overflow conditions when designing VHDL circuits.