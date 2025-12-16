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

# Tools used:
Cadance Xcelium, Genus 

# RUN DFT AND LEC CHECK:
1. DFT CHECK

•	The percentage of total registers that are scannable

<img width="903" height="591" alt="image" src="https://github.com/user-attachments/assets/a452cf3a-dc3a-40b8-b2f1-b77f2f460b48" />

•	Scan chains reported

<img width="480" height="379" alt="image" src="https://github.com/user-attachments/assets/d5b80b82-269d-44ab-b0f6-22100e48849e" />

•	Schematic view of the design

<img width="975" height="505" alt="image" src="https://github.com/user-attachments/assets/b3364d9a-e544-4d69-9768-4f6780c9372f" />

2. LEC CHECK:

•	Report key points are equivalent.

<img width="826" height="558" alt="image" src="https://github.com/user-attachments/assets/c1efff01-c1e4-4d3a-bf01-2d5d2baa6ea2" />

•	Verification report

<img width="802" height="607" alt="image" src="https://github.com/user-attachments/assets/ff7955a8-6ee5-4321-8e22-2d14dc6ff6a9" />

•	Compare revised vs. golden netlist files

<img width="975" height="739" alt="image" src="https://github.com/user-attachments/assets/9fa8a25b-a97d-4bc9-9618-5074b4aa0476" />

# Explanation:
Complete DFT and LEC check with no detect error, every comparation and result are comeback as expect.

# Tools used:
Cadence Genus and Conformal


# FLOORPLAN
Moving to one of the most important step of the design, in this stage, we added 2 pins, scan_in and scan_out

<img width="975" height="681" alt="image" src="https://github.com/user-attachments/assets/b6100f9e-90fb-44f6-b023-25943916598f" />

# POWERPLAN
Continue with Floorplan we build up Powerplan

<img width="975" height="681" alt="image" src="https://github.com/user-attachments/assets/fc267e8b-167c-45dd-97ec-c1d078f1a705" />

# PLACEMENT, CTS, AND ROUTING
I'm combining these step together because it came in a series but usually you can do it seperately. In my opinon, this stage is the most complicated.

<img width="975" height="690" alt="image" src="https://github.com/user-attachments/assets/54b49a4c-5001-4e3a-a945-b7003e84eceb" />

# FINAL STAGE:
We generate out .gds file (include everything from the beginning) and ready to send out for foundary.

# Interpretation: 
Successfully generated an up/down counter design using Cadance

# Tools used:
Cadance Innovus.








