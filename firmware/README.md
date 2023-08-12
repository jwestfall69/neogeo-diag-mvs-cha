# Firmware
The firmware for the CPLDs was written using [WinCUPL](https://www.microchip.com/en-us/products/fpgas-and-plds/spld-cplds/pld-design-resources).  WinCUPL will compile the .pld files into into .jed file.

Converting the .jed file to in the .svf is handled by [ATMISP](https://stageapps.microchip.com/design-centers/programmable-logic/spld-cpld/tools/software/atmisp).  In this program create a new "chain", select the CPLD model, JTAG Instruction: program/verify, and then pick the .jed file.

Then on the right hand side check the Write SVF file box, select the output .svf file to write, then press the RUN button.  This should generate the .svf file based on the  input .jed file.
