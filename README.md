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
add the library path
Use the command .ac dec 20 .1 1T to set up your AC analysis
Run the simulation to analyze the frequency response

# DC analysis
![image](https://github.com/user-attachments/assets/4865be51-2e38-4479-b764-5bd6b6cfd749)

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

![image](https://github.com/user-attachments/assets/8dae782a-a83c-4881-8bc3-2e60171c75ff)

# AC Analysis
Change the parameter as shown below

![image](https://github.com/user-attachments/assets/21353781-b747-4f0a-8ab5-6e52be261e88)

Waveform of ac analysis

![image](https://github.com/user-attachments/assets/240577fe-04ae-428e-b057-577bc0014cc1)

# Transient analysis
 Go to the simulation settings in LTspice, set the stop time to 1ms, and run the simulation
 The waveform of Transient Analysis

![image](https://github.com/user-attachments/assets/a2e3affc-a4c6-4ea7-80e6-6eb5808b0104)

# Result

By adjusting the sizes of the MOSFETs, M1 and M2, we achieved the desired current: M1 with a length of 500nm and width of 950nm, and M2 with a length of 300nm and width of 1020nm. The circuit had a gain of 3.8 dB and a phase shift close to 180 degrees, aligning with our expectations. It also showed stable and reliable performance when responding to changes in input

# Inference
The DC sweep analysis determined the input DC voltage.
By adjusting the MOSFET sizes, we calculated the drain current during the simulation.
Both M1 and M2 were modified to achieve the required drain current.
For the AC analysis, the AC amplitude was set to 1 to ensure accurate evaluation.
The DC sweep also displayed the Voltage Transfer Characteristic (VTC) curve at the output






















