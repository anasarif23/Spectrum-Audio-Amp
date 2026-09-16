## Version 0

The first version of the schematic, completed while learning KiCad fundamentals. This version has some design mistakes that I identified during review, including [add specifics if you can — e.g. incorrect regulator pinout, missing decoupling capacitors, etc.]. I used Claude as a learning resource throughout this stage to understand regulator behavior, KiCad's schematic tools, and best practices for power supply design.

📄 See `Advanced Audio Amplifier Schematic.pdf` for the full Version 0 schematic.

## Version 1

A revised, cleaner version of the schematic with the Version 0 mistakes corrected and the overall layout better organized. This version is still in progress — the schematic is further along, and I'm now working on completing the full PCB layout.

🖼️ See `Audio Amplifier Version 1.png` for the current schematic.

## Version 2

The PCB layout stage — all components have been placed on the board. Routing has not started yet; that's the next step.

📄 See `Audio_Amplifier.pdf` for the schematic and `Audio_Amplifier PCB FULL LAYOUT.pdf` for the current component placement.

🖼️ See `Audio_Amplifier 3D-PIC.png` for a 3D render of the board as placed so far.

---

## Bill of Materials (from schematic)

### Active Components

| Ref | Part | Description |
|-----|------|--------------|
| U1, U6–U13 | NE5532 | Dual op-amp — used across the pre-amp stage and the 7 gyrator filter bands |
| U2 | LM317-TO220 | Adjustable positive linear regulator |
| U3 | LM337-TO220 | Adjustable negative linear regulator |
| U4 | LM2596S-5 | Switching buck regulator (5V rail) |
| U5 | LMC835N | Graphic equalizer IC |
| U14 | MSGEQ7 | 7-band spectrum analyzer IC |
| U15 | Teensy 4.1 | Microcontroller |
| U16 | SN74AHCT125N | Quad buffer / 3.3V logic level shifter |
| U18 | PAM8403D | Class-D speaker amplifier |
| PS1 | DCWN03A-12 | Isolated DC-DC converter |
| D1 | 1N5822 | Schottky diode |
| D2–D9 | LED | Status/indicator LEDs |
| SW1–SW7 | Rotary Encoder | 7-band control knobs |
| RV1 | 10k | Potentiometer |
| L1 | 33µH | Inductor (buck regulator) |
| FB1 | Ferrite Bead | EMI suppression |
| J1 | SJ-3523-SMT | Audio input jack |
| J2 | Barrel Jack | 12V power input |
| J3, J4 | Screw_Terminal_01x02 | Power/output connections |
| J6 | Conn_01x06 | Pin header |

### Passives

Roughly 96 resistors (R1–R96) and 110 capacitors (C1–C110) make up the gyrator filter networks (tuned for the 63Hz–16kHz bands), op-amp gain/bias networks, and decoupling/filtering throughout the board. Full reference-designator values are in the schematic (`Audio_Amplifier.pdf`).

---

## Status

🚧 **In progress** — schematic complete (Version 1); PCB component placement complete (Version 2), routing still to be done.

## Tools Used

- KiCad (schematic capture, PCB layout)
- NE5532 dual op-amps (pre-amp and gyrator filter stages)
- LM317 / LM337 adjustable linear regulators, LM2596S-5 switching regulator
- MSGEQ7 spectrum analyzer IC, LMC835N graphic equalizer IC
- Teensy 4.1 microcontroller
- PAM8403D class-D amplifier

## What I Learned

Iterating between Version 0 and Version 1 taught me to catch design errors early through review rather than discovering them at the prototyping stage — a habit I now apply to every new project. I also used Claude as a learning tool throughout this project to fill gaps in my coursework, particularly around regulator dropout behavior and KiCad workflow, then applied that understanding directly to my design decisions.
