# Traffic Light Controller — Logisim-Evolution

A digital traffic-light controller designed in Logisim-Evolution as a coursework project, built to practice control-unit/datapath design and digital logic.

## Design
The circuit is split into three subcircuits:
- **Control Unit** — takes `RESET`, `CLK_In`, and `CAR_DETECT` as inputs and manages the timing/state logic
- **Datapath** — connects the control unit's outputs to the output stage
- **Sanitizer** — the output stage, driving 6 LEDs (`HL_in`, `FL_in` inputs) representing the light states

Internally, the design uses a ROM lookup table, a counter, registers, and comparators to sequence the light states.

## How to open
1. Install [Logisim-Evolution](https://github.com/logisim-evolution/logisim-evolution)
2. Open `Lab9.circ` in the app
3. Toggle the `RESET` and `CAR_DETECT` inputs and step the clock to see the outputs change

## Built with
Logisim-Evolution

## Status
Coursework project for a digital logic design course.
