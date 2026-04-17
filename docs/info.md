<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it work

Explain how your project works

## How to test

To ensure the reliability of the custom RISC-V SoC, I am implementing a multi-stage testing procedure on the FPGA. The process begins with verifying the UART Bootloader's ability to write binary data into the BRAM correctly. Once the memory is initialized and the 'ready' signal is active, I synchronize the system reset to the negative edge of the clock to prevent timing violations. Finally, I use SignalTap to monitor the QSPI communication, ensuring the CPU fetches instructions accurately from the virtual ROM without any signal contention.

## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any.
