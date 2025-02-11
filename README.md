# sata 3.3v injector

## Background
I came across these sata 16GB drives that I could not read or write to with a standard USB to SATA adaptor.

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-16gb-front.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-16gb-back.png" width="300"> 

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/usb-sata-cable.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-pinouts.png" width="300">

Apparently both the 5v and 3.3v supplies were required to achive this. So I thought I would design an adaptor to solve this issue.

## Schematic and PCB
My goto schematic capture and pcb design software is Kicad but I could not find suitable footprints for the sata connectors. I couldn't be bothered making them from scratch either :).

So I used easyEda for the first time wich had an Cloud based and Desktop client available.

The schematic has the male and female sata connectors connected pin to pin, except for the 3.3v line which is switched either pin to pin or to the 3.3v regulator output.

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/schematic.png">

## Fabrication


