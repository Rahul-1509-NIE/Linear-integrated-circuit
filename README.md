# Experiment - 1
Question: Given the power as P=100µw, Perform AC, DC and Transient analysis for the given circuit design by using Ltspice simulator.
# Circuit diagram -1
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

# DC analysis
![image](https://github.com/user-attachments/assets/1270f880-6629-4c96-acb3-e4b8d82fc3b6)
Steps for finding DC analysis is Go to simulate in LTspice, Select the dc output print and the run the simulation
# AC analysis
![image](https://github.com/user-attachments/assets/51d4eb17-4c62-4214-99b9-4b4e297456cb)
 Waveform of AC analysis of given circuit

 ![image](https://github.com/user-attachments/assets/914c0ea8-1b77-4e91-b1ce-cce7f8117d57)

 # Transient Analysis
 Go to the simulation settings in LTspice, set the stop time to 1ms, and run the simulation
 The waveform of Transient Analysis
 ![image](https://github.com/user-attachments/assets/0eb4b7d9-ade9-49c7-9a20-eb55b4ceb80c)

# Result
The DC analysis showed a drain current of 55.5 µA 
with NMOS size: Length = 175nm, Width = 178nm.

# Inference 
The drain current indicates if the MOSFET is in the saturation region, influenced by the gate-to-source voltage (VGS). Coupling and bypass capacitors affect frequency response, while the circuit’s gain depends on the MOSFET's characteristics. Adding necessary library files is crucial for simulation, and adjusting the MOSFET’s dimensions fine-tunes the drain current. Understanding these factors optimizes circuit performance.

# Circuit Diagram-2
![image](https://github.com/user-attachments/assets/cc783f44-f45a-4d29-ba80-21881dfc5061)

# Procedure
DC Sweep analysis
Go to the simulation settings, select a DC sweep analysis, input the required values as specified, and run the simulation.
![image](https://github.com/user-attachments/assets/6d74eb9e-71ec-4853-b530-0befc30d568f)

VTC curve
![image](https://github.com/user-attachments/assets/b9ec0177-884a-4178-9ec6-466c114672bc)

Change input as
![image](https://github.com/user-attachments/assets/617d833b-61f0-4289-9e03-58aa863a3aea)

Change the length and width of the NMOS and PMOS 
![image](https://github.com/user-attachments/assets/502be2df-ebd5-4fe8-9bf3-3e7e2339a684)
![image](https://github.com/user-attachments/assets/f67cc05e-8851-43f5-9ede-5f4a954b26ba)

# DC Analysis
Steps for finding DC analysis is Go to simulate in LTspice, Select the dc output print and the run the simulation

![Uploading image.png…]()














