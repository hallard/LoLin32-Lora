ESP32 WeMos LoLin32 Shield for HopeRF RFM95 RFM96 RFM98 Lora Modules
====================================================================

This shield is used to hold HopeRF [Lora module][4] Software with WeMos ESP32 LoLin32266 boards it has just few minimal features. 
- I2C Pullups placement
- Classic I2C connector with SCL/SDA and 3V3/GND reversable solder pad
- Groove I2C connector
- Placement for RFM95/96/98 Lora module
- Placement for choosing single Wire, SMA or u-FL Antenna type 
- 1 x WS2812B Type LED for visual indication
- Custom switch on GPIO2
- Added footprint for Microchip 24AA02E64 64 bits serial number 
- Teleinfo (French SmartMeteric Interface)



You can find more information on WeMos on their [site][1], it's really well documented.

Detailed Description
====================

Look at the schematics for more informations.

SPI connexion is classic (MOSI/MISO/CLK), 


Other pins that may need be adapted into code (for example if you use TTN network gateway code) according to the following pinout


```
Lolin32      RFM9x Module
  IO19  <----> MISO
  IO23  <----> MOSI
  IO18  <----> CLK
  IO27  <----> DIO0
  IO26  <----> DIO1
  IO4   <----> DIO2
  IO25  <----> DIO5
  IO5   <----> SEL 
  IO35  <----> Reset 

Lolin32      Shield Feature
  IO22  <----> I2C SCL
  IO21  <----> I2C SDA
  IO13  <----> WS2812 LEDS
  IO15  <----> Push Button
```

Schematic  
=========
![schematic](https://raw.githubusercontent.com/hallard/LoLin32-Lora/master/pictures/LoLin32-Lora-sch.png)  

Firmware  
========
[firmware](https://github.com/hallard/LoLin32-Lora/tree/master/firmware)  

Boards  
======
<img src="https://raw.githubusercontent.com/hallard/LoLin32-Lora/master/pictures/LoLin32-Lora-top.png" alt="Top">&nbsp;
<img src="https://raw.githubusercontent.com/hallard/LoLin32-Lora/master/pictures/LoLin32-Lora-bot.png" alt="Bottom">

You can order the PCB of this board at [PCBs.io][3] if you do so, PCBs.io give me discount that allow me to buy some new created boards.

Assembled boards (V1.0)
=======================

TBD   

License
=======

<img alt="Creative Commons Attribution-NonCommercial 4.0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png">   

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/)    
If you want to do commercial stuff with this project, please contact [CH2i company](https://ch2i.eu/en#support) so we can organize an simple agreement.

Misc
====
See news and other projects on my [blog][2] 
 
[1]: http://www.wemos.cc/wiki/doku.php?id=en:d1_mini
[2]: https://hallard.me
[3]: https://PCBs.io/share/zvZjL
[4]: http://www.hoperf.com/rf_transceiver/lora/
[5]: https://github.com/hallard/ESP-1ch-Gateway/
[6]: https://github.com/matthijskooijman/arduino-lmic/pull/34