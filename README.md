# Frequency-divider-mixed-signal-using-sky130nm

This repository presents the design of frequency divider implemented using sky130nm eSim open source EDA tool.

# Table of Contents

- [Abstract](#Abstract)
- [Introduction](#Introduction)
- [Astable Multivibrator](#Astable-Multivibrator)
- [MOD-4 Counter](#MOD-4-Counter)
- [Frequencydivider](#Frequency-divider)
	- [REFERENCE WAVEFORM](#REFERENCE-WAVEFORM)
- [Tools Used](#Tools-Used)
	- [eSim](#eSim)
	- [Makerchip](#Makerchip)
- [Pre-Layout Schematics and Simulations](#Pre-Layout-Schematics-and-Simulations)
	- [Schematics](#Schematics)
	- [Verilog](#Verilog)
	- [Oscillator (or) Astable multivibrator Circuit Details](#Oscillator-(or)-Astable-multivibrator-Circuit-Details)
	- [Frequency divider Schematicl](#Frequency-divider-Schematic)
- [Simulations](#Simulations)
	- [Astable multivibrator Waveform](#Astable-multivibrator-Waveform)
	- [Frequency divider Waveform](#Frequency-divider-Waveform)
- [Netlist of the Circuit](#Netlist-of-the-Circuit)
	- [Steps to run generate NgVeri Model](#steps-to-run-generate-ngveri-model)
	- [Steps to run this project](#steps-to-run-this-project)
- [References](#references)
- [Acknowledgement](#acknowledgement)
- [Author](#author)

# Abstract:
An electrical circuit known as a frequency divider splits a given frequency by an integer value of n. The input frequency is divided by four using a divide-by-4 circuit in this instance. An astable multivibrator and a divide-by-4 counter make up the two components that make up the frequency divider. RF devices, communication, frequency synthesizers, and other audio-based systems all depend on frequency dividers.

A divide-by-4 counter and an astable multivibrator make up the Frequency Divider. A clock signal with a particular frequency is generated by the astable multivibrator and used as an input by the counter. The counter then generates an output signal with a frequency that is divided. In this, all processes have been carried out of a CMOS-based frequency divider using Open-Source Software eSim, etc.


# Introduction:
The bit rates used by serial data transmission systems today range from 10 to 40 Gb/s. Most modern communication integrated circuits (ICs) use GaAs, InP, or SiGe bipolar technology. There have been some high-speed CMOS chips disclosed, confirming that CMOS is a good solution for designing broadband circuits since cutting-edge circuit approaches and cutting-edge fabrication processes can be combined to increase speed limitations. The lower production costs, higher yield, and integrated density make this strategy very cost-effective. frequency divider in IBM 130nm CMOS is presented. The manufactured nMOS transistors have a ft of 100 GHz. All subcircuits of this frequency divider use current-mode logic (CML) with differential signals


# Astable Multivibrator
A free-running multivibrator is another name for the astable multivibrator. It possesses two quasi-stable states, and state shifts can be produced without the use of an outside stimulus. The length of time that each state of the circuit will last is determined by the component values. Typically, an astable multivibrator is employed to create a square wave as it alternates between two states. The resistance and capacitor values in this circuit determine the time period. Additionally, it is influenced by the op-upper amps and lower threshold voltages

# MOD-4 Counter
A binary divider with an inverted output terminal that is connected back to the data terminal in a feedback loop is known as a Divide-By-4 counter. It is made up of two D flip flops. It is an asynchronous counter where each subsequent flip-flop is clocked by the output of the flip-flop before it, with the initial flip-flop being clocked by the external clock pulse. It takes some time at each stage as the signal moves in a ripple pattern, resulting in the lower frequency at the output.
 
 
# Frequency divider:

We create a straightforward yet powerful general analytical formula to calculate the frequency deviations across the entire network. The theoretical foundation and reasoning for the suggested formula.

## Rationale:
Synchronous machine rotor speeds fluctuate during a transient that is brought on by a significant disturbance, such as the occurrence of a fault and its clearance. It is generally known that each machine exhibits local non-dominant modes as well as interarea oscillation modes shared by its coherent group during a transient. The crucial argument is that because machine frequencies are not equal throughout the transient, the frequency cannot be the same throughout the system. However, only the frequencies - effectively, the rotor speeds of the internal electromotive forces (emfs) of synchronous machines can be estimated by using the temporal integration of the power system model due to the usual approximations of the standard transient stability model.


</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/106176740/194713435-36ba7aaa-817c-4c14-bb7a-2caff1d678ee.png"></br>
   fig.3: Frequency divider 
</p>

## REFERENCE WAVEFORM
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/106176740/194714728-6dea4534-1697-4b6d-9e21-a2f08eeb59c0.png"></br>
   fig.5: Frequency divider REFERENCE WAVEFORM 
</p>


# Tools Used:

## eSim:
[eSim](https://esim.fossee.in/home) is a CAD tool that helps electronic system designers to design, test and analyse their circuits. But the important feature of this tool is
that it is open source and hence the user can modify the source as per his/her need. The software provides a generic, modular and extensible platform for experiment with
electronic circuits. This software runs on all Ubuntu Linux distributions and some flavours of Windows. It uses Python, KiCad and Ngspice.
  The objective behind the development of eSim is to provide an open source EDA solution for electronics and electrical engineers. The software should be capable of performing
schematic creation, PCB design and circuit simulation (analog, digital and mixed signal). It should provide facilities to create new models and components. The architecture of
eSim has been designed by keeping these objectives in mind.

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156241968-207d738d-9245-4e82-b101-2c957cfb3b17.png"></br>
  Fig.6: eSim open source EDA tool
</p>

<b>• KiCad to Ngspice converter:</b></br>
&emsp;Analysis parameters, and the source details are provided through this module. It also allows us to add and edit the device models and subcircuits, included in the circuit
schematic. Finally, this module facilitates the conversion of KiCad netlist to Ngspice compatible ones.

[Ngspice](http://ngspice.sourceforge.net/docs.html) is a general purpose circuit simulation program for nonlinear dc, nonlinear transient, and linear ac analysis. Circuits may
contain resistors, capacitors, inductors, mutual inductors, independent voltage and current sources, four types of dependent sources, lossless and lossy transmission lines (two
separate implementations), switches, uniform distributed RC lines, and the five most common semiconductor devices: diodes, BJTs, JFETs, MESFETs, and MOSFET.

## Makerchip:
[Makerchip](https://www.makerchip.com/) Circuit design has been a game for big industry for far too long! Makerchip provides free and instant access to the latest tools from
your browser and from your desktop. This includes open-source tools and proprietary ones. Turning the tables for the open-source community, Redwood EDA, LLC's commercial
capabilities are often available for open-source development here first--*before* they are available commercially!

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156244458-943e8799-d7b3-4cdf-8906-2ff8dda606f7.png"></br>
  Fig.7: Makerchip
</p>

<b>• Verilog:</b></br>
&emsp;Verilog is a Hardware Description Language; a textual format for describing electronic circuits and systems. Applied to electronic design, Verilog is intended to be used
for verification through simulation, for timing analysis, for test analysis (testability analysis and fault grading) and for logic synthesis

[Verilator](https://www.veripool.org/verilator/): It is a tool which converts Verilog code to C++ objects.

# Pre-Layout Schematics and Simulations:

## Schematics:

### Verilog
```
   
module gaurav_kumar ( clk,out_clk );

output out_clk;

input clk ;

reg [2:0]m;

initial m = 0;

always @ (negedge (clk)) begin
 m <= m + 1;
end

assign out_clk = m[2];

endmodule

```
Verilog code in Makerchip IDE

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917375-83f425a3-2809-42f8-a685-073cdd42e31e.png"></br>
  Fig.8.1: 
</p>

Simulation of Verilog Code in Makerchip IDE

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917433-9a8fdd4c-b0ae-4243-bf12-274261e65602.png"></br>
  Fig.8.2: 
</p>

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917453-e5e917a5-c0ac-4882-b2a0-90c2393965e8.png"></br>
  Fig.8.3:
</p>

Simulation of Verilog Code in Makerchip IDE when it takes any random value by it's own

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917473-351bda5c-756f-4f27-9ae7-7035925245f6.png"></br>
  Fig.8.4: 
</p>

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917515-69137660-99e0-4f69-8321-3db7c4171b25.png"></br>
  Fig.8.5: 
</p>

This is the Simulation of Verilog Code in Makerchip IDE when the user gives value according to the requirement .

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917565-17e49081-a948-46a2-9d89-90c9d2d795b6.png"></br>
  Fig.8.6: 
</p>

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156917575-4e6c9761-b232-4582-965b-6b00b31b22cf.png"></br>
  Fig.8.7: 
</p>

### Oscillator (or) Astable multivibrator Circuit Details:


</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/157047244-aeea0b25-455c-4203-a47d-f16b92225e69.jpg"></br>
  Fig.9: Astable multivibrator circuit
</p>



### Frequency divider Schematic:

An oscillator, or astable multivibrator, is the device in question. The circuit alternates between two states as a result of the cross-coupling of the two transistors. A base current can flow when Q's base is around one diode drop above ground in one state. This maintains Q in saturation mode and keeps it turned on, allowing current to flow through the collector, maintaining a low collector voltage, and discharging C1. Because Q's base voltage is insufficient to turn it on, it is turned off.

When Q2 is turned on, a current flows through its collector, dropping the collector voltage (the amount of charge on C1) as the collector current into Q1 charges C1.

![ci](https://user-images.githubusercontent.com/106176740/194724215-559081a4-017a-4dc8-9860-150cedc7f297.jpg)

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/106176740/194724215-559081a4-017a-4dc8-9860-150cedc7f297.jpg"></br>
  Fig.11: Frequency Divider circuit
</p>


## Simulations:
### Astable multivibrator Waveform:
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/156940261-f4438a17-bed3-48a0-8c82-1a7253084a8d.jpg"></br>
  Fig.15:  8x3 Priority encoder Waveform
</p>

### Frequency divider Waveform:

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/106176740/194724314-2a983f81-e4fd-40a9-bad9-3d600cafb712.jpeg"></br>
  Fig.16.1:  waveform(1) 
</p>

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/106176740/194724297-0b16ab59-207e-457c-a373-43dd63182527.jpeg"></br>
  Fig.16.2:  waveform(2)
</p>

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/106176740/194724271-daff7de1-9de5-43cf-a5cb-365d8161a263.jpg"></br>
  Fig.16.3: Frequency divider waveform(3)
</p>

# Netlist of the Circuit:

[1]. Refer to the netlist of the circuit here: <a href='Netlist_of_comparator'>Netlist_of_comparator</a>

[2]. Refer to the netlist of the circuit here: <a href='Netlist _of _8x3 _Priority_encoder'>Netlist _of _8x3 _Priority_encoder</a>

[3]. Refer to the netlist of the circuit here: <a href='Netlist_3-bit_Flash_ADC'>Netlist_3-bit_Flash_ADC</a>

## Steps to run generate NgVeri Model
1. Open eSim
2. Run NgVeri-Makerchip 
3. Add top level verilog file in Makerchip Tab
4. Click on NgVeri tab
5. Add dependency files
6. Click on Run Verilog to NgSpice Converter
7. Debug if any errors
8. Model created successfully
## Steps to run this project
1. Open a new terminal
2. Clone this project using the following command:</br>
```git clone https://github.com/Eyantra698Sumanto/XOR-XNOR-Gate.git ```</br>
3. Change directory:</br>
```cd eSim_project_files/xor_xnor```</br>
4. Run ngspice:</br>
```ngspice xor_xnor.cir.out```</br>
5. To run the project in eSim:

  - Run eSim</br>
  - Load the project</br>
  - Open eeSchema</br>

# References:
[1]. •	https://github.com/PatelVatsalB21/Mixed_Signal_Frequency_Divider 

[2]. http://faraday1.ucd.ie/archive/papers/freqdiv.pdf#:~:text=Frequency%20Divider%20Federico%20Milano%2C%20Fellow%2C%20IEEE%2C%20Alvaro%20Ortega%2C%C2%B4,frequency%20at%20the%20buses%20of%20a%20transmission%20system.

[3]. https://www.indiabix.com/electronics-circuits/astable-multivibrator-oscillator/

[4]. •	https://www.bing.com/search?q=frequency+divider+using+cmos&qs=n&form=QBRE&sp=-1&pq=frequency+divider+using+cmos&sc=9-28&sk=&cvid=C83C9014852142D7AF7944D39E98E2A9&ghsh=0&ghacc=0&ghpl=

# Acknowledgements:

- [eSim](https://esim.fossee.in/home)
- [Indian Institute Of Technology (IIT) Bombay](https://www.iitbombay.org/)
- [Kunal Ghosh](https://github.com/kunalg123), Founder, VSD Corp. Pvt. Ltd
- [VLSI System Design (VSD) Corp. Pvt. Ltd India](https://www.vlsisystemdesign.com/)
- [SUMANTO KAR](https://github.com/Eyantra698Sumanto)

# Author:
• Gaurav Kumar, B.Tech(ECE), Dronacharya Group of Institutions, Greater Nodia, Uttar Pradesh.
