# ESPlay Retro Emulation 

Retro Emulation Collection runs on [esplay-hardware] - and ESP32 Devices with WROVER Module (4MB PSRAM).
- Nofrendo NES Emulator for play Nintendo ROM
- GNUBoy for play GameBoy and GameBoy Color
- SMSPlusGX could play Sega Master System, Game Gear and Coleco Vision ROM



[esplay-hardware]: https://github.com/pebri86/esplay-hardware

Compiling
---------

This code is an esp-idf project. You will need esp-idf to compile it. Newer versions of esp-idf may introduce incompatibilities with this code;
for your reference, the code was tested against release/v3.2 branch of esp-idf.
edit mkrelease.sh with correct location for your mktool.
Find mktool in the base firmware in my repository.

run mkrelease.sh to compile and make an .fw file that could be flashed by base firmware bootloader. Place .fw file in esplay/firmware folder on sdcard, power on esplay device while press B button until bootloader screen appear. select .fw then A -> Start to flash firmware.

Base firmware is a modified bootloader fork from odroid-go.

ROM
--- 
Please provide ROM by yourself and place them in the appropriate folder on sdcard.
