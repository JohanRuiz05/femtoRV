<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This SoC development is based on the FemtoRV32 project, which encompasses the RISC-V core known as Quark. The single-cycle microarchitecture of Quark, consisting of fetch, decode, register read, execute, and write-back stages, stands out for its minimalist and compact structure. With the assistance of open-source tools, as OpenLane and Magic, this is a femtoRV implememtation using SPI flasg and spiRAM.

## How to test

The project use the open-source tool Xyce to test the analog circuit design of the top module (femto.v), obtained from the SPICE model of the verilog files extracted with Magic. In this way, the signals required to ensure the processor's operation were verified, particularly in terms of the SPI memory and the UART peripheral.Then, you must program an external flash memory with desired application, all communication and debug messages are displayed in UART

## External hardware

The project only uses one LED display (output) as external hardware.
