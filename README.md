# Breadboard Power Supply

A dual-output regulated power supply PCB designed in KiCad, converting a 12V barrel-jack input into safe, stable 5V and 3.3V outputs for circuit prototyping. The design includes jumper-configurable voltage selectors, screw terminals, input protection, and an LED status indicator.

This project is being developed iteratively across two versions as I improve my schematic design and PCB layout skills.

---

## Version 0

The first version of the schematic, completed while learning KiCad fundamentals. This version has some design mistakes that I identified during review, including [add specifics if you can — e.g. incorrect regulator pinout, missing decoupling capacitors, etc.]. I used Claude as a learning resource throughout this stage to understand regulator behavior, KiCad's schematic tools, and best practices for power supply design.

📄 See `Advanced Audio Amplifier Schematic.pdf` for the full Version 0 schematic.

## Version 1

A revised, cleaner version of the schematic with the Version 0 mistakes corrected and the overall layout better organized. This version is still in progress — the schematic is further along, and I'm now working on completing the full PCB layout.

🖼️ See `Audio Amplifier Version 1.png` for the current schematic.

---

## Status

🚧 **In progress** — schematic refinement complete for Version 1; PCB layout in development.

## Tools Used

- KiCad (schematic capture, PCB layout)
- LM7805 / LM317 linear voltage regulators

## What I Learned

Iterating between Version 0 and Version 1 taught me to catch design errors early through review rather than discovering them at the prototyping stage — a habit I now apply to every new project. I also used Claude as a learning tool throughout this project to fill gaps in my coursework, particularly around regulator dropout behavior and KiCad workflow, then applied that understanding directly to my design decisions.
