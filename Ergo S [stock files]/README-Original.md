# VOID Ergo S
*A handwired split keyboard, running QMK firmware*

![VOID Ergo S](https://i.imgur.com/aQ571vc.jpg)

| ![](https://i.imgur.com/X6qhLW8.jpeg) 	| ![](https://i.imgur.com/vaoo9bM.jpeg) 	| ![](https://i.imgur.com/nWaW7JV.jpeg) 	|
|---------------------------------------	|---------------------------------------	|---------------------------------------	|

###### More renders [here](https://imgur.com/a/ki1BZij)

The VOID Ergo S is a 3d printed, handwired, split keyboard with a layout similar to the Iris/Corne/Kyria, running QMK Firmware on Pro Micro controllers. Connection between the two halves of the keyboard is made with an aux cable via serial.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed but recommended for the bottom cases as the ports will print with less imperfections.

The brass inserts can be fixed in the bottom case by heating them and applying pressure with a soldering iron set to about 200-220C.

*VOID Ergo S with V1 of the VOID Ergo under it*

![VOID Ergo Fat](https://i.imgur.com/liKmJqt.jpg)

# Handwiring guide

I've also put together a pretty visual handwiring guide for the VOID9, that you can browse over [here](https://victorlucachi.ro/journal/void9-wiring-guide/).

| ![](https://i.imgur.com/MHTt02w.jpg) 	| ![](https://i.imgur.com/TzdhlCM.jpg) 	| ![](https://i.imgur.com/vTpQaXI.jpg) 	|
|---------------------------------------	|---------------------------------------	|---------------------------------------	|

# Bill of Materials

* 46 diodes (tme.eu [link](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/)/aliexpress [link](https://www.aliexpress.com/item/32729204179.html))
* 44/46 cherry mx style switches
* 24 AWG (0.2 mm2) wire
* 2 x Pro Micro (aliexpress [link](https://www.aliexpress.com/item/32902569443.html))
* 2 x EC11 Rotary Encoder (optional/aliexpress [link](https://www.aliexpress.com/item/32872039030.html) mounted to the plate using [this adapter](https://www.thingiverse.com/thing:3770166))
* 10 x M2x12 allen head screws (aliexpress [link](https://www.aliexpress.com/item/32966941844.html), 14mm overall length, 4mm diameter head)
* 10 x M2 brass inserts (aliexpress [link](https://www.aliexpress.com/item/4000585933306.html), 3.5mm outer diameter)
* 2 x PJ320A 3.5mm female audio connectors (aliexpress [link](https://www.aliexpress.com/item/32368285821.html))
* 1 x 6x6x6 push button (optional (used to reset master)/aliexpress [link](https://www.aliexpress.com/item/32960657626.html))
* hot glue for securing the Pro Micros to the bottom case (optional, but recommended) the audio connectors and the reset push button.

# Pin assignment

    ROW0    ROW1    ROW2    ROW3
    B1      B3      B2      B6
    
    
    COL0    COL1    COL2    COL3    COL4    COL5
    D4      C6      D7      E6      B4      B5


    Encoder Pad A           Encoder Pad B
    F5                      F6


    Serial Pin
    D1

*Matrix layout*

![VOID Ergo S matrix layout](https://i.imgur.com/hrN9udq.png)

# QMK Fork

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/dev_void/keyboards/handwired/void_ergo). Edit them to suit your own needs and build the firmware following the QMK docs.

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).
