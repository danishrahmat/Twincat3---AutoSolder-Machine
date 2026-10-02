# Twincat3---AutoSolder-Machine
Industrial AutoSolder machine control system featuring X/Y/Z servo motion, theta stepper control, solder dispensing, and EtherCAT CoE integration.

## Machine Overview

The AutoSolder machine consists of:

- X Axis
- Y Axis
- Z Axis
- Theta Axis
- Solder Dispenser
- Beckhoff CX7000 PLC
- EtherCAT I/O
- Servo Drives
- EL7041 Stepper Terminal

## Control System

### PLC

- Beckhoff CX7000
- TwinCAT 3
- Structured Text
- 1 ms PLC task

### Motion

X/Y/Z axes use EtherCAT CoE control.

Position feedback:

- Encoder resolution: 131072 counts/revolution
- Screw lead: 5 mm/revolution

Position conversion:

Position_mm = Encoder_Count × Screw_Lead / Encoder_Resolution

## Machine Modes

### Automatic Mode

The machine executes the programmed soldering sequence.

### Manual Mode

Individual points can be operated independently for maintenance
and troubleshooting.

Example:

- P1 → Execute P1 sequence
- P2 → Execute P2 sequence
- P3 → Execute P3 sequence
- P4 → Execute P4 sequence

## Safety

The machine includes:

- Emergency stop
- Servo enable control
- Axis limit monitoring
- Position monitoring
- Fault detection
- Machine reset

## Development

Software:

- TwinCAT 3
- Beckhoff PLC
- EtherCAT
- CoE
- Structured Text

## Project Status

🚧 In Development
