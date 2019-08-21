# ESP-EASY-CAN
Information and configuration of esp-easy.pl in can module R2S2.

Pinout:
<BR><BR>
RELAY1-K1-L1=GPIO 13
<BR>
RELAY2-K2-L2=GPIO 4
<BR>
SWITCH1-S1-GPIO14
<BR>
SWITCH2-S2-GPIO12
 <BR>
I2C-SCL-GPIO2 / OR ADDTIONAL SWITCH, THERMOMENTER ETC. 
<BR>
I2C-SDA-GPIO5 / OR ADDTIONAL SWITCH, THERMOMENTER ETC. 
<BR><BR>
  
TOP:
<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/IN%20CAN%20CONECTION%20V2.0.png" alt="IN CAN MODULE V2.0">

BOTTOM:
<img src="https://github.com/Bobsonkz/ESP-EASY-CAN/blob/master/IN%20CAN%20CONECTION%20V2.0%20-%20BOTTOM.png" alt="IN CAN MODULE V2.0">

Supla instlation:
1. Find out how much eeprom memory has your ESP8266 module.
- V2.0 version with ESP07 chip have 1MB of eeprom memeory.
2. Flash blank image to ESP8266 
3. Flash Supla incan-easy image
4. Find a new Supla WiFi network nearby
5. Congirue your project
