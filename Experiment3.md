# Differential Amplifier
##   Problem statement : Design differential amplifier for the folowing Specification Vdd=3.2V , P<=2.8mw, Vicm=1.6v , Vocm=1.7v , Vp=0.6v. Perform DC analysis , Transient Analysis , Frequency Response & Extract the required parameter
1.Consider Rss
2.Replace Rss by Current Source
3.Replace Current Source By MOSFET

## Aim:
To Design differential amplifier for the folowing Specification Vdd=3.2V , P<=2.8mw, Vicm=1.6v , Vocm=1.7v , Vp=0.6v. Perform DC analysis , Transient Analysis , Frequency Response & Extract the required parameter
## Differential Amplifier - Theory

A differential amplifier operates by amplifying the voltage difference between its two input signals while rejecting common-mode signals. It uses a pair of matched transistors and a constant current source to ensure that the output is dependent solely on the differential input voltage. The differential gain is the ratio of the output voltage to the difference between the input voltages, and the common-mode rejection ratio (CMRR) measures its ability to reject common signals. This configuration makes differential amplifiers ideal for applications requiring high precision and noise rejection
The output voltage is proportional to the difference between the two input voltages.

Working:
If both the inputs receive the same siganl (common-mode signal), the ideal differential amplifier suppresses it.
The gain of the amplifier depends on the circuit configuration and reisistor values.
Vout = Ad (V1-V2)
Here Ad is differential gain

## Design 
![image](https://github.com/user-attachments/assets/90c40c8b-9c48-4952-aeed-d9413f23347e)

## Procedure:
1.Open the LTspice software, merge the library file for getting accurate values of NMOS.

2.Select the components which are needed to us like for circuit 1 we need 3.43k & 685 ohm  resistor,2 CMOSN, three voltage sources(1.6v,3.2v),ground from the components list.

3.Place them all components in necessory way which is helpfull, connect all the components as in given circuit .

4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.

5.Lets do the DC Analysis first by opting a simulation, we get .op so after placing it we will get the values of it, thet will displayed.

6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.

7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform (1.2,50m,1T),after that select the AC simulation from the given options of simulation after giving values of (Decade,20,01,1T). So we will get a output after placing node to output waveform

## Circuit Diagram-1 (Consider Rss)
![image](https://github.com/user-attachments/assets/e96fa21c-6051-4444-82bb-c5eccdd6fbbf)

Circuit is Designed as per given power and other parameters as mentioned in problem statement and circuit design is mentioned in design 
## DC Analysis

![image](https://github.com/user-attachments/assets/43080b2f-e02a-4ad2-b4a6-fb8ad9577c6f)












