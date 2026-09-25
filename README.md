# Digital Countdown Timer

A digital countdown timer implemented using discrete digital electronics components, including an NE555 timer, CD4510 BCD counters, CD4511 BCD-to-7-segment drivers, logic gates, switches, and four 7-segment displays.

## Project Overview

The project implements a multi-digit digital countdown timer using a 555 timer as the clock source, BCD counters for counting, BCD-to-7-segment drivers for display, and logic gates for control functions.

The timer supports presetting and countdown operation, with an output alert when the countdown reaches 00.

## Key Features

- Multi-digit digital countdown
- NE555-based clock generation
- BCD counting using CD4510 counters
- 7-segment display driving using CD4511 ICs
- Logic-gate-based control
- Preset and reset functionality
- Output alert at countdown completion
- Physical PCB implementation
- Proteus circuit simulation

## Main Components

- NE555 Timer IC
- CD4510 BCD Up/Down Counter ICs
- CD4511 BCD-to-7-Segment Decoder/Driver ICs
- 74LS02 Logic Gates
- 74LS08 Logic Gates
- 7-Segment Displays
- Push Buttons / Switches
- Resistors and Capacitors
- PCB and connecting components

## Working Principle

The NE555 timer generates the clock signal required for the countdown operation.

The clock pulses are applied to the BCD counters. The counter outputs are connected to CD4511 BCD-to-7-segment decoder/drivers, which drive the corresponding 7-segment displays.

Logic gates are used to implement control conditions such as rollover, reset, and the output alert condition.

The timer counts down from the preset value and activates the output alert when the countdown reaches 00.

## System Flow

```text
NE555 Clock Generator
        ↓
BCD Counter Stage
        ↓
CD4511 BCD-to-7-Segment Driver
        ↓
7-Segment Display
        ↓
Logic Control
        ↓
Output Alert
```
digital-countdown-timer/
│
├── docs/
│   └── Digital Countdown Timer Report.pdf
│
├── hardware/
│   ├── PCB_Implementation_Normal_condition.png
│   └── PCB_Implementation_Output_alert_at_00.png
│
├── simulation/
│   ├── Proteus_Circuit Diagram_Countdown_Timer.png
│   └── Countdown_Timer_Schematic_Proteus - Simulation.pdsprj
│
└── README.md
