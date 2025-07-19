 # 7-Segment Display Decoder Using Verilog HDL

This project demonstrates the design and simulation of a 7-segment display decoder using Verilog Hardware Description Language (HDL). The decoder accepts a 4-bit binary input and generates a 7-bit output to drive a common cathode 7-segment display. Each combination of input values from 0 to 9 activates the appropriate segments to display the corresponding decimal digit.

## Description

The module uses a combinational logic approach with a case statement to map binary inputs to segment patterns. For simulation and verification, ModelSim was used to observe the segment outputs as waveform signals based on different binary inputs.

The design was written in Verilog HDL and is intended for use in digital systems that require numeric display outputs.

## Files Included

- `seven_seg_decoder.v` – Verilog source code for the 7-segment decoder.
- `output_waveform.png` – Screenshot of the waveform simulation showing input and output behavior.
- `README.md` – Project description and documentation.

## Tools Used

- Verilog HDL
- ModelSim (Mentor Graphics) for simulation
- GitHub for version control

## How to Run the Simulation

1. Compile the Verilog module in ModelSim using `vlog seven_seg_decoder.v`.
2. Load the design with `vsim work.seven_seg_decoder`.
3. Add signals to the waveform using `add wave *`.
4. Force input values (e.g., `force bin 4'b1001`) and run the simulation with `run 10ns`.
5. Observe the corresponding 7-bit output for the segment.

## Output Example

For input `bin = 4'b1001` (decimal 9), the output `seg` is `7'b1111011`, which correctly activates the segments required to display the digit 9 on a 7-segment display.

## Project Status

The module was simulated successfully in ModelSim. The waveform output matches the expected results for all inputs from 0 to 9.

