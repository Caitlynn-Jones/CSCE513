# CSCE513

Advanced Computer Architecture

First project in CSCE513 asks to create a 4-bit carry lookahead adder in SystemVerilog. Two modules were created to do this.

The first module is the carry_lookahead_adder. There are two, 4-bit input signals (the operands), and two 1-bit input signals (the carry in and ctrl). If the ctrl = 0, signals the adder to add. If the ctrl = 1, signals the adder to subtract. There is a 4-bit output for the result of add/sub and a 1-bit carry out output signal.

The second module is the add_sub_4b module. It takes in the same inputs andd outputs as the carry_lookahead_adder module. The use of an xor function is used to complement each bit for input b if the ctrl = 1. The carry_lookahead_adder is then instantiated within this module to do the actual calculations

Testbench was created to test a variety of cases, all passed.
