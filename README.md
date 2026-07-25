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

## 11. Two-Level Lamp Switching with a 555

A manufacturer needs a way to alternate between two lamp settings of different output — one equivalent to three LEDs, the other to five. A single ordinary switch is the only control the user gets, so the circuit itself has to handle the toggling logic. Build it around a 555 timer.

## 12. Four-Stage Sequencer for a Production Line

A plant supervisor needs the four operations his machine performs to fire in a fixed order rather than at random. Build a circuit that issues a trigger signal to each of the four stages one after another, cycling through them in sequence. Use 555 timers together with a few basic components.

## 13. Alternating LED Groups with a CD4017

Starting from a clock source that ticks once per second, use a CD4017 decade counter to drive two banks of LEDs so that they flash back and forth — one bank on while the other is off, swapping on every pulse.

_Note: the original Arabic ("كل مجموعتين") is slightly ambiguous — most likely alternating between two groups, but possibly stepping through several groups two at a time._

## 14. Race Start Countdown

Build a starting-signal circuit for a race. It counts down through three, two, one, and then gives the "go" indication — a drag-strip style light tree, where each stage holds for a fixed interval before advancing to the next.

_Note: the output stage is left open — three sequential LEDs plus a final one, a 7-segment showing the digits, or a countdown with an audible tone at the start. A 555 clock feeding a CD4017 would cover it._

## 15. Clap-Activated Lamp

A client wants a saleable consumer product: a lamp toggled by hand claps. Each clap flips the lamp to the opposite state — on becomes off, off becomes on. A microphone-based sound detector supplies the trigger, and a CD4017 handles the toggling.

_Note: the CD4017 is a ten-stage counter being used for a two-state job, so reset it after the second step to make it divide by two. The harder part in practice is the front end — the sound detector needs enough conditioning to fire once per clap rather than several times on one sharp transient._

## 16. Clap-Controlled LED Dimmer

An extension of the clap-lamp idea, now with multiple brightness levels instead of a simple toggle. Each clap advances the LED through a four-state cycle: off, full brightness, medium, dim, then back to off. As before, a sound sensor provides the trigger and a CD4017 tracks which state you're in — but here three of its outputs each need to produce a different current through the LED rather than just switching it.

## 17. Thermostat for a Domestic Water Heater

A company wants the cheapest possible control board for an electric household water heater. Design a simple thermostat built around a Schmitt trigger, adding a relay and whatever basic components you need. The switching thresholds are deliberately separated: the heater cuts out once the water passes 60°C and switches back on when it falls to around 40°C.

_Note: that 20°C gap is the point of the exercise — the hysteresis is what stops the relay from chattering around a single set point, and the Schmitt trigger is where you set it._

## 18. Boost-Driven LED Flashlight

Put the oscillator and step-up converter material to practical use. Design a handheld torch powered by a single 3.7 V lithium cell that drives a string of six white LEDs wired in series.