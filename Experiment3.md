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

![image](https://github.com/user-attachments/assets/e3119c55-9cd8-4b83-bf65-a9a00c247ea0)  ![image](https://github.com/user-attachments/assets/5aba15da-277c-4674-b19c-7661b1e0510b)
### For W=2.52um , L=180nm We observed the Required Output By comparing the DC operationg point And design , appropriately these two parameters value is matched

## Transient Analysis
Change specification of the Sources.
### Input Waveform
![image](https://github.com/user-attachments/assets/f5a8fdad-6eac-42b4-9cd8-8ee6dfea8786)

### Output Waveform
![image](https://github.com/user-attachments/assets/de4421c6-31ae-46fb-906b-17c364c61dc4)


### Input and Output Waveform

![image](https://github.com/user-attachments/assets/cf040352-180a-4503-8c46-ed5e22a45e59)


## Gain Calculation

![image](https://github.com/user-attachments/assets/05840b9f-46d1-431a-aec8-74da6aeb546b)

## AC analysis

![image](https://github.com/user-attachments/assets/e3172a53-89c8-4486-a28e-cb8723158ffa)
Gain in AC analysis is 10.5dB , The calculation of gain in Transient analysis is 10.52dB


## Circuit Diagram-2  (Consider Current source )
![image](https://github.com/user-attachments/assets/a8076eda-5ba7-4450-bc13-59c3b9edf7cb)

Circuit is Designed as per given power and other parameters as mentioned in problem statement and circuit design is mentioned in design 
## DC Analysis

![image](https://github.com/user-attachments/assets/e0b2bf48-7d21-424d-8e04-848ef455cd04)

### For W=2.52um , L=180nm We observed the Required Output By comparing the DC operationg point And design , appropriately these two parameters value is matched

## Transient Analysis
Change specification of the Sources.
### Input Waveform
![image](https://github.com/user-attachments/assets/29e370de-cde5-4aed-9c70-97e20a3d0d2f)


### Output Waveform
![image](https://github.com/user-attachments/assets/5dcc189f-564d-4a9d-ab02-4f42549c0023)



### Input and Output Waveform

![image](https://github.com/user-attachments/assets/8443aafd-743b-4d1b-8ddb-644847fb6ac1)



## Gain Calculation

![image](https://github.com/user-attachments/assets/05840b9f-46d1-431a-aec8-74da6aeb546b)

## AC analysis

![image](https://github.com/user-attachments/assets/e83e6828-df1e-4c66-a33d-b1fcc7f48665)

Gain in AC analysis is 10.5dB , The calculation of gain in Transient analysis is 10.52dB


## Circuit Diagram-3 (Consider MOSFET As Current Source)
![image](https://github.com/user-attachments/assets/b713411d-9ee0-49cf-8f5c-fd312c8e76f8)


Circuit is Designed as per given power and other parameters as mentioned in problem statement and circuit design is mentioned in design 
## DC Analysis

![image](https://github.com/user-attachments/assets/ba2f7136-dc94-4bc1-9aaf-4dbd96f2bdc4)

### For CMOS M1,M2 W=2.58um , L=180nm & CMOS M3- W=6.22u , L=180nm  with  0.966v gate voltage
We observed the Required Output By comparing the DC operationg point And design , appropriately these two parameters value is matched

## Transient Analysis
Change specification of the Sources.
### Input Waveform
![image](https://github.com/user-attachments/assets/2f9f5b31-c871-4069-a6a4-d67039587d19)


### Output Waveform
![image](https://github.com/user-attachments/assets/fafb7e70-1753-4d4c-a321-71f3da30e7b3)



### Input and Output Waveform

![image](https://github.com/user-attachments/assets/c047b21f-7796-4ec5-89d9-8150d71cf37b)



## Gain Calculation

![image](https://github.com/user-attachments/assets/05840b9f-46d1-431a-aec8-74da6aeb546b)

## AC analysis
![image](https://github.com/user-attachments/assets/5f95976b-3974-44e6-a278-a12a4efcc910)

Gain in AC analysis is 10.5dB , The calculation of gain in Transient analysis is 10.52dB

## Conclusion 
In differencial Amplifier Specification Vdd=3.2V , P<=2.8mw, Vicm=1.6v , Vocm=1.7v , Vp=0.6v
DC analysis  For W=2.52um , L=180nm We observed the Required Output By comparing the DC operationg point and given specification
Transient Analysis , We Calculated gain and its is compared with AC analysis output waveform.
All the design specification is appeared in Simulation

## Inference 
Given power and other Specification is designed and it is simulated using LTspice.

Differential Gain – The amplifier provides significant gain for differential signals, confirming its suitability for applications requiring precise signal amplification.

Proper biasing ensures stable operation, and any variations in resistor values or transistor parameters influence the gain.

Practical Limitations – Small deviations from theoretical values were observed due to component tolerances, non-ideal transistor characteristics, and power supply variations.
We observed simulation output with given specification it is almost matched

we compared theoretical differential amplifier with practical .



