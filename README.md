# RoMCaT
MSX Rom cartridge for roms up to 64KB

This is yet another PCB design of a ROM cartridg that can hold roms up to 64 KB. Different configuration options regarargind the Z80 page (CS1/CS2/CS12) for 8, 16 and 32 KB ROMS are included using jumpers (/RD option is also available).

This design also includes the possibility of switching between LOW/HIGH 32KB pages when using 27C512 (64KB) ROMs.
The PCB is compatible with W27C256/W27C512 EEPROMs.

# Set-up

1) Solder 100nF (C2) and 4.7uF (C1) capacitors. 
2) Close Jumpers OE and SLTSL
3) Close ONLY ONE jumper (RD, CS1, CS2 or CS12) depending on the ROM configuration. Typically, CS1 and CS2 are used for 8/16KB ROMS, CS12 for 32KB ROMs. RD is usually connected for 64KB ROMs.
4) Set A15 jumper for 32 or 64 KB ROM (27C256 or 27C512, respectively)

*** 64 KB ROM with two 32 KB programs (0000 - 80000 / 8000 - FFFF)
1) Set the A15 jumper to 32 KB
2) Install the sliding switch to change the ROM page (A15 to Vcc / A15 to ground).
