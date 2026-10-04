# Arduino Traffic Light Controller 🚦

A simple Arduino-based traffic light controller that cycles through green, yellow, and red LEDs with predefined timing.

## Project Overview

This project demonstrates basic Arduino programming and digital output control using three LEDs.

The traffic light follows this sequence:

**Green → Yellow → Red → Repeat**

## Components

* Arduino Uno
* Green LED
* Yellow LED
* Red LED
* 3 × 220 Ω resistors
* Jumper wires
* Breadboard

## Timing

| Light     |  Duration |
| --------- | --------: |
| 🟢 Green  | 5 seconds |
| 🟡 Yellow | 2 seconds |
| 🔴 Red    | 5 seconds |

## Arduino Pins

| LED    | Pin |
| ------ | --: |
| Green  |   8 |
| Yellow |   9 |
| Red    |  10 |

Each LED is connected through a 220 Ω resistor to limit current.

## How It Works

The Arduino configures the three LED pins as outputs using `pinMode()`.

Inside the `loop()` function, `digitalWrite()` switches each LED ON or OFF. The `delay()` function controls how long each light remains active.

The sequence continuously repeats.

## Simulation

The circuit was simulated using Wokwi.

**Simulation:** https://wokwi.com/

A screenshot of the simulation is included in this repository.

## Current Status

✅ Arduino code completed
✅ Logic verified in simulation
✅ Wokwi simulation completed
⏳ Physical hardware testing not yet performed

## Skills Demonstrated

* Arduino programming
* Digital output control
* Basic embedded systems
* Circuit wiring
* LED interfacing
* Timing and sequencing
* Wokwi simulation

## Future Improvements

* Add a pedestrian crossing button
* Add a pedestrian LED signal
* Replace fixed delays with a more flexible timing system
* Build and test the circuit on physical hardware
