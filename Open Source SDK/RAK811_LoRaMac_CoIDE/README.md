# RAK811 LoRaMac CoIDE

This project was modified based on the [LoRa official node code](https://github.com/Lora-net/LoRaMac-node). Mainly used for user-independent development. This project is different from the AT command firmware. Bin files compiled with this project do not support AT commands. The version of LoRaWAN supported by this project is V1.0.0.

############## For Linux Compilation only ##################
### Install
Toolchain @ [Open Source SDK/gcc-arm-none-eabi-5_4-2016q3-20160926-linux,-d-,tar.bz2]

(e.g.: gcc-arm-none-eabi-5_4-2016q3-20160926-linux.tar.bz2)

Install with: 

	sudo tar xfvj gcc-arm-none-eabi-5_4-2016q3-20160926-linux.tar.bz2 -C /opt


Stm32Flasher @ stm32flash-0.5.tar.gz 
source: https://sourceforge.net/projects/stm32flash/

### Build
Well... just run make ... it should be OK

### Flash over USB

	stm32flash-code/stm32flash -w Debug/classA.bin -v -g 0x0 /dev/ttyUSB0

or, if you want to see some traces:

	stm32flash-code/stm32flash -w Debug/classA.bin -v -g 0x0 /dev/ttyUSB0 && screen /dev/ttyUSB0 115200

## RAK811
### chip： RAK811
#### Support CoIDE/Keil5
#### Base on semtech LoRaWAN1.0.2

The document please go to : http://www.rakwireless.com/en/download
