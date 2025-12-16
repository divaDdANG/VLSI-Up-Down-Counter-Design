# VLSI-Up-Down-Counter-Design
Developed a fully synchronous binary up/down counter with scan-enabled flip-flops, glitch-free control logic, and timing-optimized datapath; executed complete RTL-to-GDSII flow with Cadence tools (Xcelium, Genus, Conformal, Innovus, Tempus) targeting a 45nm 11-metal technology.

# Schematic view of the design: 

<img width="908" height="463" alt="image" src="https://github.com/user-attachments/assets/ece2a6cc-c4d6-4fc9-b215-767e0f66f407" />

# Synthesize circuit

<img width="975" height="585" alt="image" src="https://github.com/user-attachments/assets/50f2cc12-372b-4133-9216-f463d088c361" />

# Generated Netlist

<img width="726" height="655" alt="image" src="https://github.com/user-attachments/assets/e5ac15aa-6814-41d2-84e9-5f4151ef90b3" />

# Area Report

<img width="975" height="514" alt="image" src="https://github.com/user-attachments/assets/d729c3ec-7b36-457a-bc98-80329e182224" />

# Power Report

<img width="975" height="568" alt="image" src="https://github.com/user-attachments/assets/a2f7a18c-14e1-4dfc-8e2c-2d45c8b179a1" />

# Timing Report

<img width="985" height="616" alt="image" src="https://github.com/user-attachments/assets/bb502c0c-e3a4-44de-a797-99327872abd1" />

# Qor Report

<img width="850" height="751" alt="image" src="https://github.com/user-attachments/assets/ce72bbbb-b004-4ce4-a81a-30c8c5f2eb10" />

# Code Coverage and Interpretation:
The RTL simulation of the Up-Down Counter was successfully verified using Cadence Xcelium. The waveform shows correct up/down counting behavior with all bits of count[7:0] toggling during simulation.
-	Statement & Branch Coverage: All RTL paths were exercised — reset, up-count, and down-count — achieving 100% statement and branch coverage.
-	Toggle Coverage: All counter bits toggled between 0 and 1, giving 100% toggle coverage.
-	Functional Coverage: Both incrementing and decrementing operations were validated, confirming full functionality of the design.
-	Synthesis Verification: The Genus-generated netlist matches the RTL behavior, composed of flip-flops and combinational logic, confirming correct synthesis.

# Tools use:
Cadance Xcelium, Genus 
