EESchema Schematic File Version 2
LIBS:frequency_divider-rescue
LIBS:adc-dac
LIBS:memory
LIBS:xilinx
LIBS:microcontrollers
LIBS:dsp
LIBS:microchip
LIBS:analog_switches
LIBS:motorola
LIBS:texas
LIBS:intel
LIBS:audio
LIBS:interface
LIBS:digital-audio
LIBS:philips
LIBS:display
LIBS:cypress
LIBS:siliconi
LIBS:opto
LIBS:atmel
LIBS:contrib
LIBS:power
LIBS:eSim_Plot
LIBS:transistors
LIBS:conn
LIBS:eSim_User
LIBS:regul
LIBS:74xx
LIBS:cmos4000
LIBS:eSim_Analog
LIBS:eSim_Devices
LIBS:eSim_Digital
LIBS:eSim_Hybrid
LIBS:eSim_Miscellaneous
LIBS:eSim_Power
LIBS:eSim_Sources
LIBS:eSim_Subckt
LIBS:eSim_Nghdl
LIBS:eSim_Ngveri
LIBS:eSim_SKY130
LIBS:eSim_SKY130_Subckts
LIBS:3stcmringosci13
LIBS:smttrigger21
LIBS:frequency_divider-cache
EELAYER 25 0
EELAYER END
$Descr A4 11693 8268
encoding utf-8
Sheet 1 1
Title ""
Date ""
Rev ""
Comp ""
Comment1 ""
Comment2 ""
Comment3 ""
Comment4 ""
$EndDescr
$Comp
L gk-RESCUE-frequency_divider U9
U 1 1 634189C5
P 430600 -149250
F 0 "U9" H 433450 -147450 60  0000 C CNN
F 1 "gk" H 433450 -147250 60  0000 C CNN
F 2 "" H 433450 -147300 60  0000 C CNN
F 3 "" H 433450 -147300 60  0000 C CNN
	1    430600 -149250
	1    0    0    -1  
$EndComp
$Comp
L 3stcmringosci13 X1
U 1 1 6341906A
P 1900 2550
F 0 "X1" H 1550 3050 60  0000 C CNN
F 1 "3stcmringosci13" H 1850 2200 60  0000 C CNN
F 2 "" H 1900 2550 60  0001 C CNN
F 3 "" H 1900 2550 60  0001 C CNN
	1    1900 2550
	1    0    0    -1  
$EndComp
$Comp
L DC v1
U 1 1 6341906B
P 1300 3050
F 0 "v1" H 1100 3150 60  0000 C CNN
F 1 "DC" H 1100 3000 60  0000 C CNN
F 2 "R1" H 1000 3050 60  0000 C CNN
F 3 "" H 1300 3050 60  0000 C CNN
	1    1300 3050
	1    0    0    -1  
$EndComp
Text GLabel 2900 2200 2    60   Output ~ 0
output0
Text GLabel 2900 2450 2    60   Output ~ 0
output1
Text GLabel 2900 2750 2    60   Output ~ 0
output2
$Comp
L GND #PWR01
U 1 1 6341906C
P 1300 3750
F 0 "#PWR01" H 1300 3500 50  0001 C CNN
F 1 "GND" H 1300 3600 50  0000 C CNN
F 2 "" H 1300 3750 50  0001 C CNN
F 3 "" H 1300 3750 50  0001 C CNN
	1    1300 3750
	1    0    0    -1  
$EndComp
$Comp
L plot_v1 U2
U 1 1 6341906D
P 2700 2650
F 0 "U2" H 2700 3150 60  0000 C CNN
F 1 "plot_v1" H 2900 3000 60  0000 C CNN
F 2 "" H 2700 2650 60  0000 C CNN
F 3 "" H 2700 2650 60  0000 C CNN
	1    2700 2650
	-1   0    0    1   
$EndComp
$Comp
L smttrigger21 X2
U 1 1 6341906E
P 4550 2550
F 0 "X2" H 4300 2850 60  0000 C CNN
F 1 "smttrigger21" H 4550 2400 60  0000 C CNN
F 2 "" H 4550 2550 60  0001 C CNN
F 3 "" H 4550 2550 60  0001 C CNN
	1    4550 2550
	1    0    0    -1  
$EndComp
Wire Wire Line
	1300 3500 1300 3750
Wire Wire Line
	1300 2400 1300 2600
Wire Wire Line
	2500 2200 2900 2200
Wire Wire Line
	2500 2450 2900 2450
Wire Wire Line
	2500 2750 2900 2750
Wire Wire Line
	4050 2350 3600 2350
Wire Wire Line
	3600 2350 3600 1950
Wire Wire Line
	3600 1950 2750 1950
Wire Wire Line
	2750 1950 2750 2200
Connection ~ 2750 2200
$Comp
L plot_v1 U1
U 1 1 6341906F
P 2550 2000
F 0 "U1" H 2550 2500 60  0000 C CNN
F 1 "plot_v1" H 2750 2350 60  0000 C CNN
F 2 "" H 2550 2000 60  0000 C CNN
F 3 "" H 2550 2000 60  0000 C CNN
	1    2550 2000
	1    0    0    -1  
$EndComp
Wire Wire Line
	2550 1800 2550 2200
Connection ~ 2550 2200
Wire Wire Line
	1300 2550 50   2550
Wire Wire Line
	50   2550 50   4250
Wire Wire Line
	50   4250 4050 4250
Wire Wire Line
	4050 4250 4050 2550
Connection ~ 1300 2550
$Comp
L plot_v1 U3
U 1 1 63419070
P 3200 2550
F 0 "U3" H 3200 3050 60  0000 C CNN
F 1 "plot_v1" H 3400 2900 60  0000 C CNN
F 2 "" H 3200 2550 60  0000 C CNN
F 3 "" H 3200 2550 60  0000 C CNN
	1    3200 2550
	0    1    1    0   
$EndComp
Wire Wire Line
	3400 2550 2600 2550
Wire Wire Line
	2600 2550 2600 2450
Connection ~ 2600 2450
Wire Wire Line
	2700 2850 2700 2750
Connection ~ 2700 2750
$Comp
L plot_v1 U5
U 1 1 63419071
P 5250 2450
F 0 "U5" H 5250 2950 60  0000 C CNN
F 1 "plot_v1" H 5450 2800 60  0000 C CNN
F 2 "" H 5250 2450 60  0000 C CNN
F 3 "" H 5250 2450 60  0000 C CNN
	1    5250 2450
	1    0    0    -1  
$EndComp
Text GLabel 5450 2450 2    60   Output ~ 0
clk
Wire Wire Line
	5150 2450 5450 2450
Wire Wire Line
	5250 2250 5250 2450
Connection ~ 5250 2450
$Comp
L SKY130mode scmode1
U 1 1 63419072
P 1400 5150
F 0 "scmode1" H 1400 5300 98  0000 C CNB
F 1 "SKY130mode" H 1400 5050 118 0000 C CNB
F 2 "" H 1400 5300 60  0001 C CNN
F 3 "" H 1400 5300 60  0001 C CNN
	1    1400 5150
	1    0    0    -1  
$EndComp
$Comp
L adc_bridge_1 U6
U 1 1 63419A03
P 6500 2500
F 0 "U6" H 6500 2500 60  0000 C CNN
F 1 "adc_bridge_1" H 6500 2650 60  0000 C CNN
F 2 "" H 6500 2500 60  0000 C CNN
F 3 "" H 6500 2500 60  0000 C CNN
	1    6500 2500
	1    0    0    -1  
$EndComp
$Comp
L dac_bridge_1 U7
U 1 1 63419AAF
P 9050 2500
F 0 "U7" H 9050 2500 60  0000 C CNN
F 1 "dac_bridge_1" H 9050 2650 60  0000 C CNN
F 2 "" H 9050 2500 60  0000 C CNN
F 3 "" H 9050 2500 60  0000 C CNN
	1    9050 2500
	1    0    0    -1  
$EndComp
Text GLabel 10000 2500 2    60   Output ~ 0
clk_output
Wire Wire Line
	5900 2450 5900 2600
Wire Wire Line
	5900 2600 5350 2600
Wire Wire Line
	5350 2600 5350 2450
Connection ~ 5350 2450
Wire Wire Line
	9600 2450 10000 2450
Wire Wire Line
	10000 2450 10000 2500
$Comp
L plot_v1 U8
U 1 1 63419CB5
P 9750 2450
F 0 "U8" H 9750 2950 60  0000 C CNN
F 1 "plot_v1" H 9950 2800 60  0000 C CNN
F 2 "" H 9750 2450 60  0000 C CNN
F 3 "" H 9750 2450 60  0000 C CNN
	1    9750 2450
	1    0    0    -1  
$EndComp
Wire Wire Line
	9750 2250 9750 2450
Connection ~ 9750 2450
$Comp
L gaurav_kumar U4
U 1 1 6341B9D1
P 4900 4350
F 0 "U4" H 7750 6150 60  0000 C CNN
F 1 "gaurav_kumar" H 7750 6350 60  0000 C CNN
F 2 "" H 7750 6300 60  0000 C CNN
F 3 "" H 7750 6300 60  0000 C CNN
	1    4900 4350
	1    0    0    -1  
$EndComp
$EndSCHEMATC
