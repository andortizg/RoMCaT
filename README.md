# RoMCaT

## WARNING: This PCB version is not yet tested!

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
1) Set the corresponding jumper to 32 KB
2)  change the ROM page (A15 to Vcc / A15 to ground - HI/LO jumper).


# Disclaimer
--------------


Copyright © (2020) Andrés Ortiz. All rights reserved.
Redistribution without modification only for personal use is permitted, provided that the following conditions are met:

Redistributions of schematics and gerber files must retain the above copyright notice, this list of conditions and the following disclaimer.
Redistributions in PCB form must reproduce the copyright text, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THE HARDWARE IS PROVIDED “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS HARDWARE, EVEN IF ADVISED OF
THE POSSIBILITY OF SUCH DAMAGE.


