# D-flipflop
Construction of the D flip flop using vivado software 
Project Overview
This repository contains the RTL design and testbench for a standard D (Data) Flip-Flop, implemented and simulated using Xilinx Vivado. The D Flip-Flop is a fundamental synchronous sequential logic circuit that captures the value of the data input (D) on the active edge of the clock cycle and outputs it to Q.

Features

     Positive edge-triggered clocking

     Synchronous active-high reset

     Synthesizable RTL design

Truth TableClock 
    (CLK)Reset (RST)Data (D)Output (Q)Output (Q_bar)Rising Edge1X01Rising Edge0001Rising Edge011

File Structure

    d_flip_flop.v - The main design source file containing the RTL module.

    tb_d_flip_flop.v - The simulation testbench file used to verify the functional logic.

    constraints.xdc - The Xilinx Design Constraints file for FPGA pin mapping (only required if programming a physical board).

Software Requirements

    Xilinx Vivado Design Suite

    Standard text editor or Vivado built-in editor

Vivado Simulation Instructions

    Open Vivado and click Create Project.

    Select the appropriate FPGA part number or board if you intend to synthesize the design later.

    Add d_flip_flop.v to your Design Sources.

    Add tb_d_flip_flop.v to your Simulation Sources.

    Navigate to the left-hand Flow Navigator panel.

    Click Run Simulation and select Run Behavioral Simulation.

    Observe the generated waveform window to verify that the Q output updates to the value of D on the rising edge of the clock, and resets to 0 when RST is asserted.
