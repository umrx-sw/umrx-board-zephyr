# Zephyr board support for BST Application Board 3.0 / 3.1

(**Unofficial**) [Zephyr](https://www.zephyrproject.org/) board support package (BSP) 
 for [Application Board 3.1](https://www.bosch-sensortec.com/software-tools/tools/application-board-3-1/) or 
[3.0](https://www.bosch-sensortec.com/software-tools/tools/application-board-3-0/) hardware.

Repository provides board defitions to get started developing firmware using 
[zephyr RTOS](https://github.com/zephyrproject-rtos/zephyr)
(and possibly nordic [nrfconnect-sdk](https://www.nordicsemi.com/Products/Development-software/nRF-Connect-SDK)).

## How to use

When building the Zephyr firmware, specify:
* the path to the repository in the `BOARD_ROOT environment variable.
* the board name with the `-b` / `--board` frag, e.g.:
```bash
BOARD_ROOT=/path/to/umrx-board-zephyr west build -b bosch_application_board_3_0 -d build
```