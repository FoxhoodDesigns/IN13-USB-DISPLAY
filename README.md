# IN13 USB Display
Designed as a companion to the Mini-Hardware-Monitor project ( https://github.com/FoxhoodDesigns/Mini-Hardware-Monitor ), a testbed for KiCad 9.0's new features and as a Evaluation project for the newer Microchip AVR DU Microcontrollers with USB interface

This project provides a trio of old Soviet-Era IN-13 Nixie Bargraphs that can be controlled via USB CDC communication. Both as an External display OR as a Internal display (case-mod).
The board is divided into 3 parts. 
+ The boost converter that provides ~180V to ignite the IN13 tubes
+ a set of three Voltage-controlled Current sinks to manipulate the strength of the signal to the tube based on the duty cycle of a PWM input
+ A AVR64DU32 Microcontroller handling USB-communication, PWM output and potential Sensor interface via QWIIC/STEMMA-QT interface.

# Current Status
Figuring out how to set the AVR64DU as CDC USB device via Microchip MCC kit. Once done the PCB's can be sent out.
