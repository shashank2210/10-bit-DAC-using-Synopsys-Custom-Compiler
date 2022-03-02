# 10-bit-DAC-using-Synopsys-Custom-Compiler
## **ABSTRACT**
Digital to Analog Converter(DAC) is an electronic device, often an integrated circuit, that converts a digital number into a corresponding analog voltage or current. In this project I have used bottom-up approach to design the pre-layout view of 10-bit DAC, viz, for designing n-bit DAC we need 2 sub-circuits of the (n-1)-bit DAC and a sub-circuit of switch. They are connected in such a manner that the low reference voltage of first (n-1)-bit DAC is connected to the high reference voltage of the second (n-1)-bit DAC. Output of both the DACs are given to the switch circuit such that output of first DAC is the input to the high reference voltage of the switch and output of the second DAC is the input to the low reference voltage of the switch. Output of the switch is the final analog output of the DAC.

## **INTRODUCTION**
In real world, most of the signals are analog in nature while the digital systems can understand only digital signals. Hence it becomes essential to convert real world analog signals into digital signals. This can be done using digital to analog converters(DACs). A digital to analog converter takes in digital bits as input and converts it into corresponding analog voltage.

An n-bit Digital to Analog Converter (DAC) takes in n-bit digital input and converts it into corresponding analog voltage level with respect to the reference voltage. The potentiometric DAC used in the design uses the concept of Voltage Divider. It consists of 2^N equal resistors connencted in series. The basic architecture of an N-bit potentiometric DAC is shown in the figure below.

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/N-bit-DAC.png)

## **TOOLS USED**
* Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.
* Synopsys Symbol Editor : This tool was used to get a symbolic representation of the design directly from the schematic.
* Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.
* Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

## **PRE-LAYOUT SIMULATIONS**
# **Switch**
The schematic of the switch circuit designed in the Synopsys Custom Compiler is shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/Switch%20schematic.png)

The symbol of the switch generated using Symbol Editor is shown below
![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/Switch%20Symbol.png)

The test bench of the switch is shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/Switch%20test%20bench.png)

The output waveform of the switch circuit is also shown below
![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/Switch%20waveform.png)

# **2-bit DAC**
2-bit DAC is designed using 3 switch circuits.
The schematic of the 2-bit DAC is shown below
![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/2-bit%20DAC%20schematic.png)

The symbolic representation of the 2-bit DAC is as shown below
![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/2-bit%20DAC%20symbol.png)

The test bench of the 2-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/2-bit%20DAC%20test%20bench.png)

The output waveform of the 2-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/2-bit%20DAC%20waveform.png)

# **3-bit DAC**
3-bit DAC is designed using two units of 2-bit DAC and one unit of switch as sub-circuit.
The schematic of the 3-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/3-bit%20DAC%20schematic.png)

The symbolic representation of the 3-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/3-bit%20DAC%20symbol.png)

The test bench of the 3-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/3-bit%20DAC%20test%20bench.png)

The output waveform of the 3-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/3-bit%20DAC%20waveform.png)

# **4-bit DAC**
4-bit DAC is designed using two units of 3-bit DAC and one unit of switch as sub-circuit.
The schematic of the 4-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/4-bit%20DAC%20schematic.png)

The symbolic representation of the 4-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/4-bit%20DAC%20symbol.png)

The test bench of the 4-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/4-bit%20DAC%20test%20bench.png)

The output waveform of the 4-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/4-bit%20DAC%20waveform.png)

# **5-bit DAC**
5-bit DAC is designed using two units of 4-bit DAC and one unit of switch as sub-circuit.
The schematic of the 5-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/5-bit%20DAC%20schematic.png)

The symbolic representation of the 5-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/5-bit%20DAC%20symbol.png)

The test bench of the 5-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/5-bit%20DAC%20test%20bench.png)

The output waveform of the 5-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/5-bit%20DAC%20waveform.png)

# **6-bit DAC**
6-bit DAC is designed using two units of 5-bit DAC and one unit of switch as sub-circuit.
The schematic of the 6-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/6-bit%20DAC%20schematic.png)

The symbolic representation of the 6-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/6-bit%20DAC%20symbol.png)

The test bench of the 6-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/6-bit%20DAC%20test%20bench.png)

The output waveform of the 6-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/6-bit%20DAC%20waveform.png)

# **7-bit DAC**
7-bit DAC is designed using two units of 6-bit DAC and one unit of switch as sub-circuit.
The schematic of the 7-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/7-bit%20DAC%20schematic.png)

The symbolic representation of the 7-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/7-bit%20DAC%20symbol.png)

The test bench of the 7-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/7-bit%20DAC%20test%20bench.png)

The output waveform of the 7-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/7-bit%20DAC%20waveform.png)

# **8-bit DAC**
8-bit DAC is designed using two units of 7-bit DAC and one unit of switch as sub-circuit.
The schematic of the 8-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/8-bit%20DAC%20schematic.png)

The symbolic representation of the 8-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/8-bit%20DAC%20symbol.png)

The test bench of the 8-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/8-bit%20DAC%20test%20bench.png)

The output waveform of the 8-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/8-bit%20DAC%20waveform.png)

# **9-bit DAC**
9-bit DAC is designed using two units of 8-bit DAC and one unit of switch as sub-circuit.
The schematic of the 9-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/9-bit%20DAC%20schematic.png)

The symbolic representation of the 9-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/9-bit%20DAC%20symbol.png)

The test bench of the 9-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/9-bit%20DAC%20test%20bench.png)

The output waveform of the 9-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/9-bit%20DAC%20waveform.png)

# **10-bit DAC**
10-bit DAC is designed using two units of 9-bit DAC and one unit of switch as sub-circuit.
The schematic of the 10-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/10-bit%20DAC%20schematic.png)

The symbolic representation of the 10-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/10-bit%20DAC%20symbol.png)

The test bench of the 10-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/10-bit%20DAC%20test%20bench.png)

The output waveform of the 10-bit DAC is as shown below

![](https://github.com/shashank2210/10-bit-DAC-using-Synopsys-Custom-Compiler/blob/main/10-bit%20DAC%20waveform.png)


## **NETLIST**

*  Generated for: PrimeSim
*  Design library name: sm_dac_new
*  Design cell name: sm_10bit_dac_new_tb
*  Design view name: schematic
.lib '/PDK/SAED_PDK32nm/hspice/saed32nm.lib' TT

*Custom Compiler Version S-2021.09
*Tue Mar  1 12:54:37 2022

.global gnd!
********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_dac_switch
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_dac_switch vdda vout vrefh vrefl vssa din
xm10 vout net44 vrefl vssa n105 w=0.1u l=0.03u nf=1 m=1
xm11 vout net58 vrefh vssa n105 w=0.1u l=0.03u nf=1 m=1
xm3 net58 net44 vssa vssa n105 w=0.1u l=0.03u nf=1 m=1
xm0 net44 din vssa vssa n105 w=0.1u l=0.03u nf=1 m=1
xm8 vout net44 vrefh vdda p105 w=0.1u l=0.03u nf=1 m=1
xm13 vout net58 vrefl vdda p105 w=0.1u l=0.03u nf=1 m=1
xm2 net58 net44 vdda vdda p105 w=0.1u l=0.03u nf=1 m=1
xm1 net44 din vdda vdda p105 w=0.1u l=0.03u nf=1 m=1
.ends sm_dac_switch

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_2bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_2bit_dac_new vdda vout vrefh vrefl vssa d0 d1
xi2 vdda vout net16 net17 vssa d1 sm_dac_switch
xi1 vdda net17 net27 vrefl vssa d0 sm_dac_switch
xi0 vdda net16 net21 net23 vssa d0 sm_dac_switch
r7 net27 vrefl r=200
r5 net23 net27 r=200
r4 net21 net23 r=200
r3 vrefh net21 r=200
.ends sm_2bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_3bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_3bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2
xi1 vdda net19 net23 vrefl vssa d0 d1 sm_2bit_dac_new
xi0 vdda net18 vrefh net22 vssa d0 d1 sm_2bit_dac_new
xi2 vdda vout net18 net19 vssa d2 sm_dac_switch
r3 net22 net23 r=200
.ends sm_3bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_4bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_4bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3
xi1 vdda net21 net24 vrefl vssa d0 d1 d2 sm_3bit_dac_new
xi0 vdda net20 vrefh net23 vssa d0 d1 d2 sm_3bit_dac_new
xi2 vdda vout net20 net21 vssa d3 sm_dac_switch
r3 net23 net24 r=200
.ends sm_4bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_5bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_5bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3 d4
xi1 vdda net23 net26 vrefl vssa d0 d1 d2 d3 sm_4bit_dac_new
xi0 vdda net22 vrefh net25 vssa d0 d1 d2 d3 sm_4bit_dac_new
xi2 vdda vout net22 net23 vssa d4 sm_dac_switch
r3 net25 net26 r=200
.ends sm_5bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_6bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_6bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3 d4 d5
xi1 vdda net25 net28 vrefl vssa d0 d1 d2 d3 d4 sm_5bit_dac_new
xi0 vdda net24 vrefh net27 vssa d0 d1 d2 d3 d4 sm_5bit_dac_new
xi2 vdda vout net24 net25 vssa d5 sm_dac_switch
r3 net27 net28 r=200
.ends sm_6bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_7bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_7bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3 d4 d5 d6
xi1 vdda net27 net31 vrefl vssa d0 d1 d2 d3 d4 d5 sm_6bit_dac_new
xi0 vdda net26 vrefh net29 vssa d0 d1 d2 d3 d4 d5 sm_6bit_dac_new
xi2 vdda vout net26 net27 vssa d6 sm_dac_switch
r4 net29 net31 r=200
.ends sm_7bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_8bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_8bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3 d4 d5 d6 d7
xi1 vdda net29 net32 vrefl vssa d0 d1 d2 d3 d4 d5 d6 sm_7bit_dac_new
xi0 vdda net28 vrefh net31 vssa d0 d1 d2 d3 d4 d5 d6 sm_7bit_dac_new
xi2 vdda vout net28 net29 vssa d7 sm_dac_switch
r3 net31 net32 r=200
.ends sm_8bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_9bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_9bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3 d4 d5 d6 d7 d8
xi1 vdda net31 net34 vrefl vssa d0 d1 d2 d3 d4 d5 d6 d7 sm_8bit_dac_new
xi0 vdda net30 vrefh net33 vssa d0 d1 d2 d3 d4 d5 d6 d7 sm_8bit_dac_new
xi2 vdda vout net30 net31 vssa d8 sm_dac_switch
r3 net33 net34 r=200
.ends sm_9bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_10bit_dac_new
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sm_10bit_dac_new vdda vout vrefh vrefl vssa d0 d1 d2 d3 d4 d5 d6 d7 d8
+ d9
xi1 vdda net33 net36 vrefl vssa d0 d1 d2 d3 d4 d5 d6 d7 d8 sm_9bit_dac_new
xi0 vdda net32 vrefh net35 vssa d0 d1 d2 d3 d4 d5 d6 d7 d8 sm_9bit_dac_new
xi2 vdda vout net32 net33 vssa d9 sm_dac_switch
r3 net35 net36 r=200
.ends sm_10bit_dac_new

********************************************************************************
* Library          : sm_dac_new
* Cell             : sm_10bit_dac_new_tb
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
xi0 net17 vout net17 gnd! gnd! d0 d1 d2 d3 d4 d5 d6 d7 d8 d9 sm_10bit_dac_new
v1 net17 gnd! dc=1.8
c2 vout gnd! c=5p
v11 d9 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 100u 200u )
v10 d8 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 80u 160u )
v9 d7 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 70u 140u )
v8 d6 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 60u 120u )
v7 d5 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 50u 100u )
v6 d4 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 40u 80u )
v5 d3 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 30u 60u )
v4 d2 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 20u 40u )
v4_1 d1 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 10u 20u )
v3 d0 gnd! dc=0 pulse ( 0 1.05 0 0.1u 0.1u 5u 10u )








.tran '1u' '250u' name=tran

.option primesim_remove_probe_prefix = 0
.probe v(*) i(*) level=1
.probe tran v(vout) v(d0) v(d1) v(d2) v(d3) v(d4) v(d5) v(d6) v(d7) v(d8) v(d9)

.temp 25



.option primesim_output=wdf


.option parhier = LOCAL






.end


## **CONCLUSION**
The conversion of digital input to analog output is thus shown in this project. Moreover the design flow is also maintained by adding schematic view followed by conversion to symbol further followed by the test bench using the symbol and finally using the PrimeWave to generate the output waveform of the test bench.

## **AUTHOR**
Shashank Mishra, Jadavpur University

## **ACKNOWLEDGEMENT**
* Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd. - kunalpghosh@gmail.com
* Chinmay panda, IIT Hyderabad
* Sameer Durgoji, NIT Karnataka
* Synopsys Team/Company

## **REFERENCES**
* Sameer Durgoji's video
* Inderjit Singh Dhanjal's YouTube video
