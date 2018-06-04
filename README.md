# Dual 6X03 Adapter Schematic and Printed Circuit Board v1.0
This PCB will allow the use of two different 6X03 variants in a 6803-based system.  Only one CPU can be active at any time, and the CPU must be selected before boot.

## Theory
The 6X03 device can operate in modes 6801 configuration mode 2 or 3 only.  Essentially, Expanded Multiplexed mode with or without ROM.  At this moment, it is unclear how many of the 6X03 pins are tristated during RESET, so I took the safe approach of placing all known output lines (Address, Data, AS, E, R/W), and a few lines known to be outputs on the TANDY MC-10 (the first target of this PCB) to ensure operation.  If testing proves all lines to be in tristate or read state during RESET, I will simplify the schematic.

## License
Copyright (C) 2018  Jim Brain, RETRO Innovations

These files are free designs; you can redistribute them and/or modify
them under the terms of the Creative Commons Attribution-ShareAlike 
4.0 International License.

You should have received a copy of the license along with this
work. If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.

These files are distributed in the hope that they will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
license for more details.

