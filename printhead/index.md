# The printhead

(If you want nice photos of the printhead, [Kobra 2 Pro Insights printhead page](https://1coderookie.github.io/Kobra2ProInsights/hardware/printhead/) has a lot!)

The new printhead is used in the Kobra 2 Pro, Plus and Max, and contains the following inside:
* A 6-wire stepper (center taps not connected to motherboard). Model is marked as **42SHDB0066Z-10WD** connected to a direct drive system.
* A 100k NTC Thermistor.
* A 24V 60W heater cartridge
* A proprietary Anycubic Volcano-style heater block, comes with a silicone sock.  
* A proprietary Anycubic Volcano-style nozzle, incompatible with a regular heatbreak. The cylindric shaped end of the nozzle fits inside the bottom end of the heatbreak's throat. 
* A heatbreak (total length 26mm, 6mm OD / 4mm ID throat, M6 thread) with a ~40mm PTFE tube.
* The heatsink fan is a 24V 30x30x10 axial fan. Model marked as **HSC BCY3010D24H**
* The part cooling fan is a 24V 50x50x20 centrifugal fan. Model is marked as **COOLCOX BF5020H24D**
* An inductive proximity sensor for "Automatic Bed Leveling". According to [1coderookie](https://github.com/1coderookie), it is a PNP-NO type, 6-36V operating voltage.  
* A distribution board that also contains an accelerometer. It is the same type of accelerometer that is being used at the bed, an LIS2DW12.

## Pinouts
![Printhead pinout](Printhead-pinout.svg)

Connectors are as follows:
* Motherboard is a 2 row x 9 pin IDC connector.
* T0, FAN0 and FAN1 are JST PH 2.0 connectors, 2 pins.
* LEVE is a JST PH 2.0 connector, 3 pins.
* HEATER is a Molex Micro-Fit 3.0 connector, 2 pins.

## Extra images
![The distribution board](./printhead_distributor.png)
