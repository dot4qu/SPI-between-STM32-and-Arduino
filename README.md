# SPI-between-STM32-and-Arduino
An example of SPI communication from an STM32 master to an Arduino slave

_Ignore the `basic\_leds` project names, I didn't want to deal with refactoring the name throughout the whole project and makefile since CubeMX wouldn't let me alter it._

### Hardware
STM32F103C8 "blue pill" Cortex-M3 and Arduino Duo. Debugger is an ST-Link/V2.

### Compiling
The default toolchain for building and debugging this project is `arm-none-eabi-gcc` and `openocd`. To compile and link, all you should need is `make`.

### Debugging
For debugging, in one terminal window run `make server` to start the openocd server and in another `make debug`. This will attach to the `openocd` gdb server according to the parameters set in `.gdbinit`.

