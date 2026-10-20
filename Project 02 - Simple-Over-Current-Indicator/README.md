# Title

## Overview
A lamp manufacturer needs a quick go/no-go test for its 12 V lamps: anything drawing more than 1 A fails. Come up with the lowest-cost circuit that turns on a red LED above that threshold and a green LED below it — essentially a one-point current comparison with a visual output.

## Components
## Component List

-   **Voltage Sources:**
    
    -   **V1:** 15V DC voltage source
        
    -   **V2:** 9V DC voltage source
        
-   **Resistors:**
    
    -   **R1:** 1kΩ
        
    -   **R2:** 10kΩ
        
    -   **R3:** 10kΩ
        
-   **Transistors:**
    
    -   **Q1:** PNP BJT
        
    -   **Q2:** NPN BJT
        
-   **Diodes & LEDs:**
    
    -   **D1:** Zener diode (BZX84C12L)
        
    -   **D2, D3, D4:** LEDs
        
    -   **D5, D6, D7:** LEDs
        
    -   **D8:** Standard diode

## Circuit Diagram

Add Fritzing or schematic image here.
![image](schematic/image.png) 

## Hardware Build

Add real breadboard photos here.

## How It Works

The Arduino reads the analog voltage from the potentiometer using an analog input pin. The value is converted into a number of LEDs to turn ON.

## Result

When the potentiometer is rotated, the LED level changes.