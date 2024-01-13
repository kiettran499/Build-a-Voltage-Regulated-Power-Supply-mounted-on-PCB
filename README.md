# Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB

<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/Full_circuit.png">

## Description

- In this project, we are required to build a Voltage Regulated Power Supply mounted on a Printed Circuit Board (PCB) which is designed in Eagle. The circuit is powered by a 18V AC input signal and has ability to transform a 3.3V DC output signal at 1A maximum load. To achieve the final output, there are some aims that we need to manage.
  -	Reducing output voltage ripple until it smaller 2%.
  -	When the circuit is overloaded (current > 2V), the switching stops.
  -	Optimize the size of capacitor as well as the size of PCB.
  -	Using snubber circuit and non-polarized film capacitor to smooth the output voltage and mitigate high frequency noise.
  -	Understanding how AC signal is transformed to wished DC signal, and how the output signal is change with various load (66Ω, 10Ω, 3.3Ω). 
  -	Understanding how to control buck converter by the IC chip, how the PWM IC chip produce signal, then provide signal to buck converter.

## Design Analysis & Calculation

- The Pulse Width Modulated Switching Voltage Regulator uses to step down the voltage when signal went through the regulator which control by Feedback Control Unit. There are 3 main parts in this circuit: Before buck converter, IC control unit and Buck converter.

- Block diagram of the whole circuit:
<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/Block%20diagram%20of%20the%20whole%20circuit.png">

- Schematic of the circuit:
<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/Schematic.png">
  
- The design of the PCB:
<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/PCB_design.png">
  
- PCB circuit board with calculated components:
<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/PCB_board.png">

- Full circuit (input, output and measurement):
<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/Full_circuit.png">
  
## Result & Conclusion

- Output Voltage is measured by Oscilloscope meter:
<p align="center">
  <img width="500" src="https://github.com/kiettran499/Build-a-Voltage-Regulated-Power-Supply-mounted-on-PCB/blob/main/Output_Voltage_by_Oscilloscope_meter.png">

- We can state that our Pulse Width Modulated Switching Voltage Regulator circuit worked as expected. It produces 3.3VDC output at the maximum load 1A. The circuit produce a very small ripple voltage (all load below 150mA). The snubber circuit has eliminated the spike in the waveform. 
