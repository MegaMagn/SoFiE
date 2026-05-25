# SoFiE: Soft Finger Exoskeleton for Intelligent Grasping
Soft, wearable, 3D printable, and modular exoskeleton.
## NOTE
This work is part of an ongoing master thesis project. Certain implementations, refinements, and code structure optimizations are still under development.

## Overview
In the repository you will find all the necessary files to print and assemble your own soft exoskeleton and control it.

## Folders and files
- Arduino_ESP32 project files
  Contains the Arduino .ino file and the .cpp and .h files for controlling and logging data on the ESP32.
- Enclosure
  Contains the .stl files used for the electronics enclosure.
- Hand
  Contains the .stl files for constructing the main glove part and an assortment of PTFE tube clamps used to secure the PTFE tubes to the glove.
- Index finger
  Contains the .stl files for contructing the index finger module of the exoskeleton. 
- ESPLogger.py
  The logging and communication script meant to run on the computer in conjunction with the exoskeleton.
- requirements.txt
  required python packages

## Hardware needed
* ESP32s 30 pin devboard
* Pololu Micro Metal Gear Motor (6V, 250:1)
* Pololu 5V Step up/Step down buck converter
* sparkFun Micro Magnetometer - MMC5983MA (Qwiic)
* 6 mm x 2 mm round Neudymium magnet
* Adafruit PCA9546 4-Channel STEMMA QT / Qwiic I2C Multiplexer
* Pololu DRV8835 Dual Motor driver
* 7.4 V, 1000 mAh, 2S LiPo battery
* 1 k Ohm resistors for StretchSense voltage divider
* Assortment of resistors, capacitors and an opAmp for current sense if wanted.

## Materials and printing
The exoskeleton is primarily printed on a Prusa MK3s and a Prusa XL 5T in red varioShore TPU from Colorfabb. It is printed using their recommended settings, at a nozzle temperature of 220°C  
The StretchSense sensor is made of Conductive Filaflex TPU from Recreus, again dried and printed using their recommended settigns on a Prusa MK3s at a nozzle temeperature of 240°C

## Environment
Python version: 3.11
Install:
py -3.11 -m venv .venv
source .venv/Scripts/activate
pip install -r requirements.txt
