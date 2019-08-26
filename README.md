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
2. Flash blank image to ESP8266 
3. Flash Supla incan-easy image
4. Find a new Supla WiFi network nearby
5. Configrue your project:
<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/EXAMPLE%20SUPLA%20CONFIG.png" alt="SUPLA CONFIG">

