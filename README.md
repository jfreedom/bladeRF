# bladeRF Source #
This repository contains all the source code required to program and interact with a bladeRF platform, including firmware for the Cypress FX3 USB controller, HDL for the Altera Cyclone IV FPGA, and C code for the host side driver, library, and command line interface.

The source is organized as follows:

| Directory                     | Description                                                                                       |
| ----------------------------- |:--------------------------------------------------------------------------------------------------|
| [common][common]              | Source and header files common across the platform                                                |
| [fx3_firmware][fx3_firmware]  | Firmware for the Cypress FX3 USB controller                                                       |
| [hdl][hdl]                    | All HDL code associated with the Cyclone IV FPGA                                                  |
| [linux][linux]                | The linux kernel driver, library and command-line interface for interacting with a bladeRF device |

## Building Procedure ##
Each subsection of the source code can be built by itself and maintains their own README files for building.  The recommended build flow is as such:

- Build FX3 firmware under [`fx3_firmware`][fx3_firmware]
- Build FPGA image under [`hdl`][hdl]
- Build linux kernel driver under [`linux/kernel`][linux_kernel]
- Build linux libbladeRF library under [`linux/lib`][linux_lib]
- Build command-line application under [`linux/apps`][linux_apps]

[common]: ./common (Common)
[fx3_firmware]: ./fx3_firmware (FX3 Firmware)
[hdl]: ./hdl (HDL)
[linux]: ./linux (Linux)
[linux_kernel]: ./linux/kernel (Linux Kernel Driver)
[linux_lib]: ./linux/lib (Linux Library)
[linux_apps]: ./linux/apps (Linux Apps)

