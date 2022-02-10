Homebrew 32bit computer
=======================

About
-----
Following after my minimal 16bit 68010 computer design
(https://github.com/jtsiomb/m68kcomputer) this is an attempt to make a much
more advanced 32bit computer, based on the Motorola 68030 CPU.

The main objective of this project is to make a stand-alone computer, capable of
running a custom UNIX system with virtual memory. The 68030 processor was chosen
because it has an on-chip MMU.

The plan is to include the following on the main board:
 - Analog video output
 - PS/2 keyboard controller
 - ATA hard drive interface for fixed storage
 - SD card for removable storage
 - 68881 floating point co-processor
 - Dual RS232 serial port
 - Battery-backed RTC

Directory structure:
 - `hw` - hardware: kicad files and pdf schematics.

Design Progress
---------------

### Main board ###
 - [X] Schematic: almost completed, minor tweaks, video left for an expansion
 - [ ] PCB layout: not started
 - [ ] Firmware: not started
 - [ ] Boot ROM monitor: not started
 - [ ] Operating system: not started

### Video expansion card ###
 - [ ] Schematic
 - [ ] PCB layout
 - [ ] OS support

### Audio expansion card ###
 - [ ] Schematic
 - [ ] PCB layout
 - [ ] OS support

License
-------
Copyright (C) 2022 John Tsiombikas <nuclear@member.fsf.org>

You are free to use, reproduce, modify, and redistribute any part of this
project, provided you make any derivative work you release, freely available
under the same terms.

Both hardware designs, and software parts of this project, are released under
the terms of the GNU General Public License v3, or at your option any later
version published by the Free Software Foundation. See `LICENSE` for details.

To comply with the license, when releasing derivative hardware designs, you
must provide the full EDA project files, GAL equation files, and of course
firmware/software source code. Releasing only images of schematics, gerbers,
JED files, and firmware binaries is *not* sufficient for compliance.
