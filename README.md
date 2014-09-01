fpganes - Port from Nexys4 to Nexys3
====================================

It's designed to run on the Nexys4 board and built with
Xilinx ISE. I've forked the project to port it to Nexys3

Use "loader" to download ROMS to it over the built-in UART.
Compile with Visual Studio 2013 update 3 or newer.
You might need to change hardcoded stuff in the loader to
point at the right COM port and joystick.
Also, you need to connect the UART USB cable to the board,
it's not the same cable you use to program it.

"loader" also transmits joypad commands from my USB joypad
to the FPGA across UART.

NB. as of the time of writing, the project doesn't actually
work, as I just got started.
