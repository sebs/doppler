# doppler hardwware

![doppler](img/dadamachines-doppler-front.png)

The doppler is a Cortex M4F Microcontroller + FPGA development board. It comes in the same tiny form factor similar to a [Teensy](https://www.pjrc.com/store/teensy35.html) and is open source. 

## Features
- 120Mhz ARM Cortex M4F MCU 512KB Flash (Microchip ATSAMD51G19A) with FPU
- FPGA 5000 LUT, 1MBit RAM, 6 DSP Cores,OSC, PLL (Lattice ICE40UP5K)
- Arduino IDE compatible
- Breadboard friendly (DIL48)
- Micro USB
- Power over USB or external via pin headers
- VCC 3.5V …. 5.5V 
- All GPIO Pins are 3.3V
- 1 LED connected to SAMD51
- 4 x 4 LED Matrix (connected to FPGA)
- 2 User buttons (connected to FPGA)
- AREF Solder Jumper
- I2C (need external pullup), SPI, QSPI, USART Pins 
- 2 DAC pins, 10 ADC pins
- Pinout here: https://github.com/dadamachines/doppler/blob/master/hardware/doppler-quickstart_print.pdf
- Full open source toolchain
- SWD programming pin headers
- Double press reset to enter the bootloader
- [UF2 Bootloader](https://github.com/Microsoft/uf2-samdx1) with Firmwareupload via simple USB stick mode (Mass Storage Device)

