# ESP-EASY-CAN
Information and configuration of esp-easy.pl in can module R2S2.

<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/R2S2%20V2.0%20Board.jpg" alt="IN CAN MODULE V2.0" width="300">

<br>
Pinout:

Pin name   | Primary function        | Additional function         |
-----------|-------------------------|-----------------------------|
 GPIO 13   | RELAY1-K1-L1            | No                          | 
 GPIO 4    | RELAY2-K2-L2            | No                          | 
 GPIO 14   | SWITCH1-S1              | No                          | 
 GPIO 12   | SWITCH2-S2              | No                          |  
 GPIO 2    |I2C-SCL                  | SWITCH, THERMOMENTER ETC    |
 GPIO 5    |I2C-SDA                  | SWITCH, THERMOMENTER ETC    |
 GPIO 1    |TX                       | SWITCH, THERMOMENTER ETC    |
 GPIO 3    |RX                       | SWITCH, THERMOMENTER ETC    |

<BR> <BR>

PCb design:
 
 TOP                                                             | BOTTOM                                                    |
-----------------------------------------------------------------|-----------------------------------------------------------|
<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/IN%20CAN%20CONECTION%20V2.0.png" alt="IN CAN MODULE V2.0" width="400">|<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/IN%20CAN%20CONECTION%20V2.0%20-%20BOTTOM.png" alt="IN CAN MODULE V2.0" width="400">|

Typical connection:

 Light bulbs                                                     | Roller shutter                                            |
-----------------------------------------------------------------|-----------------------------------------------------------|
<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/Typical%20connection%20-%20light%20bulbs.png" alt="IN CAN MODULE V2.0" width="400">|<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/Typical%20connection%20-%20roller%20shutter.png" alt="IN CAN MODULE V2.0" width="400">|
 
Supla instlation:
1. Find out how much eeprom memory has your ESP8266 module.
- V2.0 version with ESP07 chip have 1MB of eeprom memory.
2. Download ESP flasher for example <a href="http://www.14core.com/flashing-upgrade-eps8266-v1-firmware-with-espressif-flash-tool/"> Flash Download Tools Version 2.4 </a> and confirgure project like this: <img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/ESP%20FLASH%20TOOL%202.4%20SETUP.png" alt="IN CAN MODULE V2.0" width="400">

3. Flash blank image to ESP8266 and reboot esp chip  
4. Flash <a href="https://github.com/SUPLA/ESP8266/blob/master/esp_init_data_default.bin">esp_init_data_default.bin</a> acording to your memory size:

Address     | Memory size     |
------------|-----------------|
 0x7c000  | 512 kB |
 0xfc000  | 1 MB |
 0x1fc000 | 2 MB |
 0x3fc000 | 4 MB |
 0x7fc000 | 8 MB |
 0xffc000 | 16 MB |

5. Flash Supla <a href="https://github.com/Espablo/SUPLA_Firmware/tree/master/inCan_Easy">incan-easy</a>
6. Register on <a href="https://cloud.supla.org/login">SUPLA CLOUD</a>  website
6. Find a new Supla WiFi network nearby
7. Configrue your project:
<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/EXAMPLE%20SUPLA%20CONFIG.png" alt="SUPLA CONFIG">
- SET BUTTON CONFIG AS "GPIO 14" AND "10x" 
8. Connect the board according to the settings to keep the correct directions

Function    | Button          |
------------|-----------------|
DOWN        | S2,L2           |
UP          | S1,L1           |
CONFIG      | S1 (PUSCH x 10) |
