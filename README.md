# Bazz Fuss Guitar Pedal

## Project Overview
This is a classic bazz fuss circuit modeled in LTSpice and built on a solderless breadboard (KiCad schematic and PCB in progress).

## Demo
<img src="https://github.com/user-attachments/assets/aad28ed0-28ab-46fc-86cb-c2a7f88469d7" height=500 />


## Technical Specifications
- 100k Ohm resistor
- 1N914 Diode
- 100k pot and knob
- 2N5088 / MPSA13 transistors
- 10uF capacitor
- 0.1uF capacitor
- 1/4" Mono Jack (output)
- 1/4" Stereo Jack (input)
- 9V battery
  
## How It works
It's easier to think of the circuit in two phases, when the transistor is on and when it's off. 
1. When the transistor is on the effect is obvious, everything on an equipotential with it is pulled to 0V. That creates the clipping at the bottom of the waveform.
2. When the transistor is off the diode is on (the voltage at the base is low), and the voltage difference across the diode pulls the input waveform up to around 1V.

The effects are best observed by plotting the waveform at the collector of the transistor, as the capacitor at the end removes the DC.

## Design and Validation Process

1. Simulation

I first simulated the circuit in LTSpice and observed the waveform while using the simulator to develop my conceptual understanding.

Circuit Schematic | Waveform Output
--------| --------
<img width="789" height="330" alt="Screenshot 2025-08-21 at 2 09 59 PM" src="https://github.com/user-attachments/assets/817ceb6e-3f4d-47ea-b7db-d8afefec38ea" />|<img width="789" height="330" alt="Screenshot 2025-08-21 at 2 09 03 PM" src="https://github.com/user-attachments/assets/318348dd-d7f6-4693-9893-07c284bbc20d" />


2. Physical Prototype
I then breadboarded the circuit (try out both transistors)
<img src="https://github.com/user-attachments/assets/7bff8e32-b138-4808-b765-b5207097ba2b" height="300" />

## KiCad Schematic
(next steps are to make the KiCad schematic and manufacture the PCB)
