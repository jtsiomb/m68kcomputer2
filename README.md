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

This project is in the early stages, so there's not much to see here yet.

Directory structure:
 - `hw` - hardware: kicad files and pdf schematics.

License
-------
Copyright (C) 2022 John Tsiombikas <nuclear@member.fsf.org>

You are free to use, reproduce, modify, redistribute any part of this project,
provided you make any derivative work you release, freely available under the
same terms.

More specifically hardware parts of this project are released under the
Creative Commons Attribution Share-Alike license (see `LICENSE.hw` for details),
and software parts are released under the GNU General Public License v3, or
later (see `LICENSE.sw` for details).
