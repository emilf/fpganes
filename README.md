fpganes - Port from Nexys4 to Nexys3
====================================

It's designed to run on the Nexys4 board and built with
Xilinx ISE. I've forked the project to port it to Nexys3

Use "loader" to download ROMs to it over the built-in UART.
Compile with Visual Studio 2013 update 3 or newer.
You might need to change hardcoded stuff in the loader to
point at the right COM port and joystick.
Also, you need to connect the UART USB cable to the board,
it's not the same connector you use to program it.

"loader" also transmits joypad commands from my USB joypad
to the FPGA across UART.

TODO:
 * Connect either joystick to the USB host port or a NES controller via pmod. Being tied to the UART and a computer sucks.
 * Optionally embed a test game in the bit file, to get away from the UART
 * Higher quality output via a VGA port/DVI/HDMI via pmod or equivilant
 * Document the board switch, led, button and 7-seg display functionality
