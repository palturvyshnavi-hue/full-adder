# Full Adder using Verilog

## Aim
To design and simulate a 1-bit Full Adder using Verilog HDL.

## Files

- `full_adder.v` - Full Adder design
- `full_adder_tb.v` - Testbench
- `README.md` - Project documentation
- `output.txt` - Simulation output

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
|0|0|0|0|0|
|0|0|1|1|0|
|0|1|0|1|0|
|0|1|1|0|1|
|1|0|0|1|0|
|1|0|1|0|1|
|1|1|0|0|1|
|1|1|1|1|1|

## Compile

```bash
iverilog -o full_adder_sim full_adder.v full_adder_tb.v
```

## Run

```bash
vvp full_adder_sim
```

## Expected Output

```
--------------------------------
 A B Cin | Sum Cout
--------------------------------
 0 0  0  |  0    0
 0 0  1  |  1    0
 0 1  0  |  1    0
 0 1  1  |  0    1
 1 0  0  |  1    0
 1 0  1  |  0    1
 1 1  0  |  0    1
 1 1  1  |  1    1
--------------------------------
```