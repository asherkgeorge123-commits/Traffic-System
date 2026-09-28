# Traffic Light Controller — Logisim-Evolution

A digital traffic-light controller designed in Logisim-Evolution as a coursework project, built to practice control-unit/datapath design and digital logic.

## Design
- **Datapath:** two 3-bit registers (HL = highway, FL = farm road) hold the light state. A rotate unit and two multiplexers update them.
- **Control unit:** a 6-bit counter steps through a 64x5 ROM. Each 5-bit word sets the register write-enables, register select, and function. RESET returns the counter to 0; CAR_DETECT holds the sequence until a car arrives.
- **Sanitizer:** gate logic that guarantees exactly one LED per road is lit for any register value, and only lights green for the valid green state.

## How to open
1. Install [Logisim-Evolution](https://github.com/logisim-evolution/logisim-evolution)
2. Open `Lab9.circ` in the app
3. Toggle the `RESET` and `CAR_DETECT` inputs and step the clock to see the outputs change

## Built with
Logisim-Evolution

## Status
Coursework project for a digital logic design course.
