# AC-DC-Converter
A simple full-wave bridge rectifier circuit built in KiCad, converting AC input to a smoothed DC output with a power-indicator LED.

https://github.com/Manideep136/AC-DC-Converter/blob/main/images/3d.png

Overview

This project takes an AC input through screw terminal J1, rectifies it using a full-wave bridge rectifier (D1–D4, 1N4007 diodes), smooths the output with a 1000µF capacitor (C1), and outputs clean DC through screw terminal J2. A power indicator LED (D5) is driven through a voltage divider (R1: 10kΩ, R2: 2.2kΩ) to show when the circuit is powered.

Circuit Description
Component	Value	Function
D1–D4	1N4007	Full-wave bridge rectifier
C1	1000µF	Output smoothing/filter capacitor
R1	10kΩ	Current-limiting resistor for LED indicator branch
R2	2.2kΩ	Voltage divider resistor for LED indicator
D5	LED	Power-on indicator
J1	Screw Terminal (2-pin)	AC input
J2	Screw Terminal (2-pin)	DC output
Schematic

Show Image

PCB Layout

Show Image

Files
*.kicad_pro, *.kicad_sch, *.kicad_pcb — KiCad project, schematic, and PCB layout files
gerbers/ — Fabrication files (Gerber + drill files) ready to send to a PCB manufacturer
images/ — Renders and screenshots of the schematic, PCB, and 3D model
How to Use
Open AC-DC-Converter.kicad_pro in KiCad to view/edit the schematic and PCB.
To manufacture the board, send the contents of gerbers/ to your preferred PCB fab (e.g. JLCPCB, PCBWay).
Connect an AC source to J1 and take your regulated DC output from J2.
Notes
Standard 1N4007 diodes are rated for up to 1A and 1000V reverse voltage — suitable for low-power AC-DC conversion.
This is a basic rectifier without voltage regulation; add a linear regulator (e.g. 7805) downstream if a fixed regulated voltage is required.
License

Feel free to specify a license here (e.g. MIT, CERN-OHL) if you'd like others to reuse this design.
