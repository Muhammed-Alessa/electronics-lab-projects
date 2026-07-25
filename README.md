# electronics-lab-projects
Small practical electronics projects covering analog circuits, digital logic, Arduino, sensors, and mixed-signal experiments.


## 1. Automated Day/Night Aquarium Lighting System

Build lighting for a fish tank that reacts to ambient light on its own. Three LEDs are involved: the white ones should glow more strongly as daylight gets brighter, while the blue ones take over once it gets dark. Sensing is done with a small solar cell, which reaches about 15 V under full midday sun. The circuit should stay simple and use only basic components.

## 2. Simple Over-Current Indicator

A lamp manufacturer needs a quick go/no-go test for its 12 V lamps: anything drawing more than 1 A fails. Come up with the lowest-cost circuit that turns on a red LED above that threshold and a green LED below it — essentially a one-point current comparison with a visual output.

## 3. Simple Battery Voltage Monitor

Add a state-of-charge indicator to a device running from a 12 V battery. The circuit draws its own supply from that same battery and compares the terminal voltage against a 10 V threshold: green above it, red below it.

## 4. Cooling Fan Control

Design temperature-triggered switching for an engine cooling fan. Once the measured temperature climbs past the set point, the fan should turn on by itself, with no manual input.

## 5. Modified Cooling Fan Control

Revisit the previous fan circuit and add hold-over behaviour. Rather than cutting out the instant the temperature falls back, the fan should keep running for a short while afterwards before shutting down.

## 6. Secret Code Door Lock

Give a homeowner keyless entry to a room. Entry is by typing a stored passcode on a keypad, so nothing has to be carried around; a correct entry releases the lock.

## 7. DC Motor Direction Control

For a toy manufacturer, work out a way to reverse a DC motor from a joystick — pushing one way spins the motor forward, pushing the other way spins it backward.

## 8. Mailbox Detector

Let a homeowner know from indoors whether anything has arrived in the mailbox. Something dropped into the box should be detected, and an LED should then stay lit rather than flashing briefly.

## 9. Proximity Sensor with Audio Feedback

Create a parking aid that signals distance by tone instead of a display. A speaker sounds a pitch that climbs higher as the vehicle closes in on a wall. An LDR is one option for sensing the distance, though any other suitable sensor is acceptable.

## 10. Mailbox Mail Indicator — Part 2

Extend the mailbox project with a more expressive output. Instead of a single LED, drive a 7-segment display that spells out **POST** one character at a time in sequence whenever mail is detected.