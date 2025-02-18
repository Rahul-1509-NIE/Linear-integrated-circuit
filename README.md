# Experiment - 1
Question: Given the power as P=100µw, Perform AC, DC and Transient analysis for the given circuit design by using Ltspice simulator.
# Circuit diagram 
![image](https://github.com/user-attachments/assets/586bf188-a39f-4404-946b-8fd7af3d7ab9)
## We used LTspice for Creating circuit diagram
Here 2 voltage sources and 1 mosfet and 1 resistor for buildiong the circuit
# Procedure
1. Create a Folder
First things first, create a new folder and name it "project file". This will be your go-to place for all the project files.

2. Set Up Your MOSFETs
Let's configure the MOSFETs:
For the NMOS:
Name it CMOSN
Set the length (L) to 180nm
Set the width (W) to 3μm
For the PMOS:
Name it CMOSP
Set the length (L) to 180nm
Set the width (W) to 3μm

3. DC Analysis
Next, we'll perform a DC analysis:
Apply Vdd = 1.8V
Set Vgs = 0.9V
Set up a DC operating point analysis with the .op command
Run the analysis to determine Vout and Id

4. Transient Analysis
For transient analysis, follow these steps:
Set Vgs = 0.9V
Apply an amplitude of 50mV
Use a frequency of 1kHz

5. AC Analysis
Finally, let’s set up the AC analysis:
Ensure you add the library path
Use the command .ac dec 20 .1 1T to set up your AC analysis
Run the simulation to analyze the frequency response
