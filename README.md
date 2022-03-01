# XOR-Implementation-using-CMOS
XOR Gate is implemented using 28nm CMOS Technology in Synopsis Custom Design Platform

# Table of Content

- ABSTRACT
- INTRODUCTION
- TOOLS USED
- XOR Circuit Design Using CMOS
- STEP 1 - CMOS INVERTER GATE
- STEP 2 - XOR GATE
- AUTHOR
- ACKNOWLEDGEMENT
- REFERENCE

# Abstract

XOR gate (sometimes EOR, or EXOR and pronounced as Exclusive OR) is a digital logic gate that gives a true (1 or HIGH) output when the number of true inputs is odd. In this paper XOR Gate is designed using 28nm CMOS technology by using Synopsys Custom Design Platform.

# Introduction

An XOR gate implements an exclusive or from mathematical logic that is, a true output results if one, and only one, of the inputs to the gate is true. If both inputs are false (0/LOW) or both are true, a false output results. XOR represents the inequality function, i.e., the output is true if the inputs are not alike otherwise the output is false. A way to remember XOR is "must have one or the other but not both".

![image](https://user-images.githubusercontent.com/100705148/156196319-1cbcd5ac-801d-4138-88f6-a4e5269328e9.png)

XOR can also be viewed as addition modulo 2. As a result, XOR gates are used to implement binary addition in Computers. A half adder consists of an XOR gate and an AND gate. Other uses include subtractors, comparators, and controlled inverters. The algebraic expressions (A . Bbar + Abar . B ) or (A + B) (Abar + Bbar) or (A xor B) all represent the XOR gate with inputs A and B. The behavior of XOR is summarized in the truth table shown in fig 1(b).

# Tools Used

Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# XOR Circuit Design Using CMOS

The CMOS design for XOR Gate is shown in fig 2. This circuit is a 2 input XOR Gate. An XOR Gate designed using CMOS consists of combinations of PMOS and NMOS so that the desired output can be derived. Here Inverter are also used for Inverted inputs of A and B.

When both the inputs are ‘0’ both the PMOS transistor will turn ON and the sources of these PMOS are connected with input A and B, PMOS passes weak ‘0’ signal.

Now consider two cases, Inputs are distinguished, either 01 or 10. In this case one of the PMOS will turn On and passes weak 1 output.

Final Case is both inputs are ‘1’. Both the PMOS transistor will now turn OFF. Now again NMOS which represents across the output comes into picture with the diode connection and passes weak ‘0’.

![image](https://user-images.githubusercontent.com/100705148/156197765-7e8d8a60-1461-4c8d-b8ea-0b83dc014635.png)

# STEP 1 - CMOS INVERTER GATE

The CMOS design for the Inverter is shown in fig.

![image](https://user-images.githubusercontent.com/100705148/156198341-5462f4a8-5ff6-48b7-b5b9-c6444e13a1b7.png)

- Schematic 

![image](https://user-images.githubusercontent.com/100705148/156199894-6b87d960-c640-403e-b3fc-603d37fe5a21.png)

- Symbol

![image](https://user-images.githubusercontent.com/100705148/156200014-e4272612-a0f8-49a6-af2a-cd248a5e923b.png)

- TestBench

![image](https://user-images.githubusercontent.com/100705148/156200212-751dc378-c908-4c65-8b1d-8eee8a76f8ba.png)


# STEP 2 - XOR GATE 

- Schematic

![image](https://user-images.githubusercontent.com/100705148/156200784-5a2b4fde-74ba-467b-ba81-03da2428358e.png)

- Symbol

![image](https://user-images.githubusercontent.com/100705148/156200896-d2a67db5-3be6-487e-8dc6-c9eda8e0ba80.png)

- TestBench

![image](https://user-images.githubusercontent.com/100705148/156201023-51e6bb14-876f-4bbf-8f33-9c4761827251.png)

- PrimeWave

Give following inputs to check XOR Gate Output.

![image](https://user-images.githubusercontent.com/100705148/156201275-8e20ed38-def0-406b-9840-307a9a27639f.png)

- XOR Gate Waveform 

![image](https://user-images.githubusercontent.com/100705148/156201502-f07dc284-e974-4d57-b47a-300f298a8f27.png)

# AUTHOR

Raman Rajaram Surkutlawar, M.tech (Embedded System Technologies), Vellore Institute of Technology, Vellore

# ACKNOWLEDGEMENT

- Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
- Synopsys, India
- VLSI System Design(VSD) Corporation Private Limited India
- Indian Institute of Technology, Hyderabad
- Cloud Based Analog IC Design Hackathon
- Sameer Durgoji, NIT Karnataka
- Chinmay panda, IIT Hyderabad

# REFERENCES

- S. Harutyunyan, K. Safaryan, F. Aslikyan, S. Melikyan and R. Musayelyan, "Low Power Design of XOR Circuit," 2019 IEEE 39th  International Conference on Electronics and Nanotechnology (ELNANO), 2019, pp. 38-41, doi: 10.1109/ELNANO.2019.8783721.

- Meghana, Kulkarni & Sridhar, V. & G.H.Kulkarni,. (2010). The Quantized Differential Comparator in Flash Analog to Digital  Converter Design. International journal of Computer Networks & Communications. 2. 10.5121/ijcnc.2010.2404.

- https://spu.edu.sy/downloads/files/1559456069_Ch-03_Lec5_%20Logic _%20Gets.pdf
