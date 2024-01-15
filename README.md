# WLED ESP32 Christmas Board

![Kicad](https://img.shields.io/badge/KiCad-314CB0.svg?style=for-the-badge&logo=KiCad&logoColor=white) ![Home Assistant](https://img.shields.io/badge/home%20assistant-%2341BDF5.svg?style=for-the-badge&logo=home-assistant&logoColor=white) 

This board is designed to control 4 x WS2812B string lights (Max 3A Total) via WLED software, and it was added a 4A fuse to protect. Max current for the 4 strings is about 3A, and 1A is left to ESP32.   

<img src="/Images/Board.png">



Board was tested with 2 x WS2812B 5 meters string lights, each draws arround 400-600 mA with color white and brightness at 100%. WLED version was [v0.14.0 "Hoshi"](https://github.com/Aircoookie/WLED/releases/tag/v0.14.0).


<img src="/Images/Test_Circuit.png">

------------


### Schematic 

The [schematic](/PCB/Schematic.pdf) is arround ESP32 WROOM 32E microcontroler. A 4A fuse was added to protect the circuit in case of short circuit, the AMS1117 regulates the input voltage to 3.3V and powers the ESP32.

<img src="/Images/Schematic.png">

------------

### PCB

[This](/PCB) 1.6mm board contains 4 layers with the stackup Signal+Power/GND/GND/Signal+Power.The connector on the right is for programming and it works with pogo pins.  

<img src="/Images/PCB.png">


------------

### Known issues

- Some noise on TX/RX lines, sometimes [this](https://user-images.githubusercontent.com/64553282/108736433-e6be2380-7531-11eb-8186-5ca70f359cc5.PNG) appears and causes board to crash, by connecting pogo pins withot any connection to a programmer board fixed the issue


------------

### To-Do

- Fixing noise on TX/RX lines




