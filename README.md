# Implementation of 9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler
9-Stage Ring Oscillator is desined using 28nm CMOS Technology.

# Table of Content 
- Abstract 
- Introduction
- Tools Used
- Circuit Design
- Netlist
- Acknowledgement
- Reference


## Abstract

An Oscillator generates a signal with specific frequency and which is used for synchronizing the computational process in digital systems. In this project we design and do analysis of ring oscillator using 28nm technology. Ring oscillator is basically a device consisting of odd number of inverters connected in series with positive feedback. It’s output oscillates between two voltage levels either 1 or zero.

# Introduction

Ring oscillator is a type of relaxation oscillator containing odd number of inverters. The output of last inverter is connected to the first inverter which is positive feedback. The number of inverter stages depends on the frequency which we want to generate. There will be a delay due to inverter and as the stages increases the oscillator frequency will be reduced. 

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/ckt.png)



# Tools Used

- Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

- Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

- Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# Circuit Design

The CMOS design for the circuit is shown in fig. 

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/CMOSCircuit.png)

- Schematic

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/Schematic.png)

In schematic I have designed trigger circuit using transmission gates and another inverter to drive the ring oscillator circuit initially.
                                                                                                                                                                                                                                                                                                                                                                          
- Symbol

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/Symbol.png)                                                                                                                                                                                                                                                                                                                                                                               

- Testbench Schematic

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/Testbench_Schematic.png)  

- Primewave Window

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/Testsuit%20Pathway.png)  

- Testbench Waveform

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/Waveform.png)  

- Frequency and Time period measurement

![image](https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/images/Frequency%20and%20Time%20Period.png)

Transient analysis has been performed and obtained time period = 120ps or 0.12ns and Frequency = 8.33GHz

# Netlist
The netlist of the circuit has also been uploaded to the repo with the file name - netlist.txt (https://github.com/girishkumar-1997/9-Stage-Ring-Oscillator-using-Synopsis-Custom-Compiler/blob/master/netlist.txt) 

# Author
Avula Girish Kumar, MTech-VLSI and Embedded Systems , Defence Institute of Advanced Technology, Pune, Maharashtra

# Acknowledgement

- Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
- Synopsys, India
- VLSI System Design(VSD) Corporation Private Limited India
- Indian Institute of Technology, Hyderabad 
- Cloud Based Analog IC Design Hackathon
- Sameer Durgoji, NIT Karnataka
- Chinmay panda, IIT Hyderabad

# References

- 	V. Sikarwar, N. Yadav and S. Akashe, "Design and analysis of CMOS ring oscillator using 45 nm technology," 2013 3rd IEEE International Advance Computing Conference (IACC), 2013, pp. 1491-1495, 

- 	Masten, H.N. (2015). Ring oscillator design in 32 nm CMOS with frequency and power analysis for changing supply voltage. 

