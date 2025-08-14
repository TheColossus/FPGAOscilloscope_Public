# FPGA Oscilloscope

The "KM Scope" was born in the ECE241 Digital Systems course at the University of Toronto. Using the the DE1-SoC Development Board to implement a hardware-only oscilloscope, KM challenges students to push the limits of their creativity for the ECE241 Final Project. The input signal is sampled through the onboard Analog/Digitial Converter, processed in the Cyclone V FPGA chip, and the output waveform is displayed through VGA.

## Specifications

- 50 kHz refresh rate
- Dual-channel
- Up to 100kHz bandwidth
- 0.04 ms / div (horizontal axis)
- 1mV / div to 200 mV / div
- 0.000V to 4.095V input voltage
- For CH0: Rising edge trigger, falling edge trigger, event capture (HOLD)
- 320px x 240px VGA resolution

## Controls

- KEY[0] - system refresh
- KEY[1] - decrease trigger level
- SW[2:0] - select vertical scaling (mV / div):
  - 000 = 1mV
  - 001 = 10mV
  - 010 = 50mV
  - 011 = 100mV
  - 100, 110, 111 = 200mV
- SW[3] - select Falling Edge trigger
- SW[4] - select Rising Edge trigger
- SW[5] - trigger "coarse mode". 5px vs 1px trigger adjustments
- SW[6] - event capture (HOLD)
- SW[7] - no connect
- SW[8] - Enable CH0
- SW[9} - Enable CH1

## Video Demo
[![FGPA Oscilloscope Demo](https://img.youtube.com/vi/16YwXYDHad8/0.jpg)](https://youtu.be/16YwXYDHad8)
