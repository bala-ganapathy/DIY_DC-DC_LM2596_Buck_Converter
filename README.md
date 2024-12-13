# DIY DC-DC Buck Converter  
This repository contains the KiCad project files for a DIY DC-DC buck converter designed to step down a higher input voltage to a stable, lower output voltage. It is aimed at providing an efficient power solution for electronic devices requiring a specific operating voltage, such as sensors, microcontrollers, and other low-power devices.

## Project Files  
- **Schematic Diagram**: Attached 
- **PCB Layout**: Attached
## Design Overview  
This DIY DC-DC buck converter uses the **LM2596** IC, which is a highly efficient, adjustable step-down (buck) voltage regulator. The converter can take input voltages ranging from 4V to 40V and efficiently output a fixed lower voltage (such as 5V, 9V, or 12V) to power various electronics. The design is intended for low to medium power applications, with a focus on providing stable output and minimizing power loss.

### Key Features:
- **Adjustable Output Voltage**: The output voltage is adjustable by selecting the appropriate feedback resistors.
- **High Efficiency**: Using the LM2596 ensures high efficiency, typically around 80-90%, minimizing heat generation.
- **Overcurrent Protection**: Built-in protection mechanisms to prevent damage under overload conditions.
- **Compact Design**: The PCB layout is optimized for small form-factor applications, making it suitable for portable devices.

## Components  
| Component         | Value        | Purpose                                    |  
|-------------------|--------------|--------------------------------------------|  
| LM2596            | -            | DC-DC Buck Converter IC                   |  
| C_in1             | 100 µF       | Input Capacitor (for voltage stability)    |  
| C_out1            | 220 µF       | Output Capacitor (for smooth output)       |  
| C_feedback1       | 10 µF        | Feedback Capacitor (stability)             |  
| L1                | 33 µH        | Inductor (energy storage for conversion)   |  
| D1                | 1N5819       | Schottky Diode (for rectification)         |  
| R1                | 1 kΩ         | Feedback Resistor (sets output voltage)    |  
| J_input           | -            | Power Input Connector                      |  
| J_output          | -            | Power Output Connector                     |  

## Notes  
- **Voltage Adjustment**: The output voltage is adjustable by changing the feedback resistors (R1) according to the desired output voltage formula provided in the LM2596 datasheet.
- **Thermal Considerations**: The LM2596 operates efficiently, but it is still important to ensure good thermal management, especially at higher input voltages or current draws.
- **Simulation**: Currently, this design has not been simulated, so real-world testing is essential to ensure performance under various conditions.
- **No Ground Pin**: The J_ground pin is not used in this design, as the ground connection is directly routed to the PCB.

## Design Goals  
This project aims to deliver a compact and reliable power supply solution suitable for applications where high efficiency and stable voltage are essential. The converter is ideal for powering small electronics, Arduino projects, sensors, and other low-power devices requiring regulated power.
