# Agricultural Spraying Drone (Model)

A working quad-copter model of an agricultural spraying drone, built end to end: a 3D-printed frame, flight electronics, a custom Bluetooth remote, and an onboard spray tank. It is the buildable 1/10-scale model from my B.Sc. design thesis (Altınbaş University, Mechanical Engineering, 2021), taking the full-size agricultural-drone design from theory into a flying prototype.

**Stack:** quad-copter | cut-and-drilled aluminum frame (SolidWorks) | 3D-printed spray tank | Pixhawk flight controller + GPS | Bluetooth pump remote (Proteus PCB, HC-05 master/slave) | DC pump + nozzle | thrust/weight sizing (Gabriel Stempler method, cross-checked with eCalc)

https://github.com/user-attachments/assets/3429aaf9-a88a-4d7b-93ad-cc5afbd50fac

## What it is

The full agricultural spraying drone was designed in my first thesis; this project is the practical 1/10-scale model that proves the design flies and sprays. It was built across the full stack: choosing and sizing parts against a lift budget, designing and building the frame, wiring and calibrating the flight electronics, building a Bluetooth pump remote, and fitting a working spray tank, then flight-testing it.

<p>
  <img src="https://github.com/user-attachments/assets/32e66445-bc86-445f-bc28-fa67d5e3a822" width="49%" alt="Assembled spraying drone">
  <img src="https://github.com/user-attachments/assets/a3e17e7e-2f4d-4dae-bf7c-607dd9b6fabb" width="49%" alt="Drone with spray tank fitted">
</p>

## Highlights

- **Frame:** cut-and-drilled aluminum, multiple pieces fitted with plastic screws, designed in SolidWorks and sized to fit the spray tank and 10 x 4.5 in propellers (10 in for efficiency, 4.5 pitch for stability). The first frame was fully 3D-printed and shook itself apart in flight, so it was rebuilt in aluminum, a hard lesson in material limits under vibration.
- **Lift and weight sizing:** thrust-to-weight calculations using the Gabriel Stempler method, cross-checked with eCalc, to pick motors and props against the all-up weight budget.
- **Flight control:** Pixhawk flight controller with GPS, transmitter and receiver, brought up through firmware, accelerometer, and radio calibration.
- **Spray tank:** 3D-printed and sealed with dichloromethane against leaks, fed by a DC pump to a spray nozzle, with flow-rate, flight-speed, and area-coverage calculations for the spraying pattern.
- **Bluetooth pump remote:** a separate HC-05 master/slave pair that toggles the spray pump in flight, with the circuit designed in **Proteus**. The firmware was small and is not preserved here.

CAD design of the frame:

![Frame CAD](https://github.com/user-attachments/assets/ca9641b4-cf94-423e-a567-5e7f27e4fe3c)

Spray tank:

![Spray tank](https://github.com/user-attachments/assets/ebd9f392-abf5-4b83-bae4-0e8a844fa3a1)

Custom Bluetooth remote:

![Bluetooth remote](https://github.com/user-attachments/assets/fa253e5b-539f-438e-b675-bbb77e7aed60)

Thrust/weight sizing in eCalc:

![eCalc sizing](https://github.com/user-attachments/assets/039ac068-25cd-479a-9d8c-fb01190ea0a3)

## Measured (model)

| | Weight | Flight time |
|---|---|---|
| Dry | 1493 g | ~4.3 min |
| With water | 1770 g | ~3.3 min |

Water payload: 277 g. Propellers: 10 x 4.5 in. Configuration: quad-copter. Flight controller: Pixhawk.

## Scope (honest)

This is a B.Sc. design project from 2021, a 1/10-scale model built to validate a full-size agricultural-drone design, not a production aircraft. It is an academic prototype, documented in a 43-page thesis. The value here is the end-to-end build: mechanical design, flight electronics, a hand-built custom remote, and flight testing.

## Author

**Ken KADILAR** | mechatronics / embedded
Portfolio: [canarchive.com](https://canarchive.com) | [ken-kadilar](https://www.linkedin.com/in/ken-kadilar/)
