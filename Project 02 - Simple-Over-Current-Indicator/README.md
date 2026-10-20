# Title

## Overview
A lamp manufacturer needs a quick go/no-go test for its 12 V lamps: anything drawing more than 1 A fails. Come up with the lowest-cost circuit that turns on a red LED above that threshold and a green LED below it — essentially a one-point current comparison with a visual output.

## Components

## Circuit Diagram

Add Fritzing or schematic image here.
![image](.attachments/9e68fd17d351a965e2230d7d138b08b8b4343cfb.png) 

## Hardware Build

Add real breadboard photos here.

## How It Works

The Arduino reads the analog voltage from the potentiometer using an analog input pin. The value is converted into a number of LEDs to turn ON.

## Result

When the potentiometer is rotated, the LED level changes.