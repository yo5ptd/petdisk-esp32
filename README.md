# petdisk-esp32
CBM PETDISK based on Esp32 and MicroSD

## Introduction
My fourth PCB design, first (mostly) SMD one to test how ordering assembled PCB from JLCPCB works. Motivation for this was that it's a bit of a pain to order @bitfixer 's Petdisk Max V2 Esp32 from the US, and I've found no alternatives in the EU. 

## Hardware documentation

As per bitfixer's Petdisk V2 Max https://github.com/bitfixer/petdisk-max . Ports as per https://github.com/svenpetersen1965/PET-IEEE-488-Extension .

I've only changed the SD slot to Hanbo Electric TS-013 as this was available at JLCPCB.

### Schematic and PCB layout

[Schematic](CBM-Petdisk-Schematic.pdf)

[PCB Layout](CBM-Petdisk-Board.pdf)

[Assembled](images/assembled.jpg)

[Front](petdisk%20esp32.jpg)

[Back](petdisk%20esp32-back.jpg)


## Panelization and odering from JLCPCB

Panelized with Kikit addon with hand-breakable "mousebytes", it still fits the 100x100 mm JLCPCB limit (Kikit.json settings included, details in https://github.com/yaqwsx/KiKit). 

The idea is to order the placement for the cheap SMD components, and only solder 3 electrolytic capacitors, the ESP32 module and a "805 Strip Connector 3.96mm Pitch 12 Pin" connector from Aliexpress. Cost per board from JLPCB thus is around 2.7$ when ordered in batches of 5 (10 boards in total, coupons used) :) With connector, capacitors, esp32 should not get over 8.5$ per board.

You need the:
[Gerbers](gerbers.2xpetdisk-esp32.zip)

[BOM](BOM_JLCSMT.xlsx)

[CPL](JLCSMT_CPL.xlsx)

Disregards the duplicate message, also allow auto placement alignment.

## Programming

note that the programming port pinout is different from the original.

THIS BOARD IS STILL UNTESTED!
