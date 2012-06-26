stm32-template
==============

This is a simple project template for the
[STM32 Discovery](http://www.st.com/internet/evalboard/product/250863.jsp),
an evaluation board with the STM32F100RB microcontroller (128 KB Flash, 8 KB RAM).

This repository is based on [jeremyherbert/stm32-template](https://github.com/jeremyherbert/stm32-templates).

Prerequisites
-------------
 - GCC based ARM Toolchain, i.e. [Sourcery CodeBench Lite Edition](http://www.mentor.com/embedded-software/sourcery-tools/sourcery-codebench/editions/lite-edition/) or [summon-arm-toolchain](https://github.com/esden/summon-arm-toolchain)
 - STM32 Discovery programmer tool, i.e. [texane/stlink](https://github.com/texane/stlink)

Installation
------------

  1. Put all your source files `*.c` into `src/`
  2. Put all your header files `*.h` into `inc/`
  3. Add the name of every source file with its name and the `.o` extension to the `OBJS=…` line in the `Makefile`

Usage
-----

  - To compile your project and generate the corresponding `.bin` firmware, run `make`.
  - Run `make flash` to write the generated `.bin` file to the STM32 flash memory.
  - `make gdb-server` and `make gdb-client` can be used to invoke the debugger service and client.
