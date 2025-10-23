# 4-Layer Macintosh IIfx 16 MB SIMM

This repository contains a PCB layout for a 16MB SIMM to be used in
the Macintosh IIfx system.  The SIMM is a proprietary, 8 bit wide
proprietary type with 64 pins. It is based on the two-layer design,
https://github.com/hanshuebner/maciifxsimm
by Hans Hübner.

Notable changes:
* A ground plane and a partial power plane has been added.
* Signals are not routed between pins to ease hand soldering.
* Capacitors were relocated directly underneath the chips to improve bypassing.
* The ground plane was extended to some of the pins that are unused by the IIfx to optionally improve signal quality.

The design has been tested with 128MB of HM5116100AS7 chips in a repaired battery-damaged IIfx using the Snooper memory test.
Maximum overclock was 60 MHz with 5.30V, and 57 MHz with 4.97V -- the same as a factory-assembled 8MB 70ns SIMM set.


![4-Layer Macintosh IIfx 16 MB SIMM unpopulated](./images/4layer-maciifxsimm-pcb-tinned-and-caps-installed.jpg)
![4-Layer Macintosh IIfx 16 MB SIMM front](./images/4layer-maciifxsimm-front.jpg)
![4-Layer Macintosh IIfx 16 MB SIMM back](./images/4layer-maciifxsimm-back.jpg)
![4-Layer Macintosh IIfx 16 MB SIMM installed](./images/4layer-maciifxsimm-installed.jpg)

## Fabrication Notes
A set of 10 test PCBs were manufactured by JLCPCB on 2025-08-16 using the following order parameters:
Base Material:	FR-4
Layers:	4
Dimension:	97.8 mm* 22.2 mm
Delivery Format:	Single PCB
PCB Thickness:	1.2mm
Specify Stackup:	no No requirement
PCB Color:	Green
Silkscreen:	White
Via Covering:	Untented
Surface Finish:	HASL(with lead)
Deburring/Edge rounding:	Yes
Outer Copper Weight:	1 oz
Inner Copper Weight:	1 oz
Gold Fingers:	No
Electrical Test:	Flying Probe Fully Test
Castellated Holes:	no
Press-Fit Hole:	No
Edge Plating:	No
Mark on PCB	Remove Mark
Blind Slot:	No
Min via hole size/diameter:	0.3mm/(0.4/0.45mm)
4-Wire Kelvin Test:	No
Appearance Quality:	IPC Class 2 Standard
Silkscreen Technology:	Ink-jet/Screen Printing Silkscreen
Board Outline Tolerance:	±0.2mm(Regular)
Countersink Hole:	No
Backdrill:	No
Total Cost: US$87.53


With a 1.2mm board thickness and 1oz inner copper with HASL finish, the SIMMs fit well into the sockets without additional solder.

The chip spacing is enough to fit a small iron for hand soldering.
The capacitors were soldered first, then a thick coating of solder with rosin flux was placed on each pad.
The corners of the chips were soldered, then a hot plate was used to reflow the rest of the pins.

## License

This work is licensed under a Creative Commons Attribution-ShareAlike
4.0 International License. See
[https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/).

