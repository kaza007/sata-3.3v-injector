# sata 3.3v injector

## Background
I came across these sata 16GB drives that I could not read or write to with a standard USB to SATA adaptor.

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-16gb-front.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-16gb-back.png" width="300"> 

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/usb-sata-cable.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-pinouts.png" width="300">

Apparently both the 5v and 3.3v supplies were required to achive this. So I thought I would design an adaptor to solve this issue.

## Schematic and PCB
My goto schematic capture and pcb design software is Kicad but I could not find suitable footprints for the sata connectors. I couldn't be bothered making them from scratch either :).

So I used easyEda for the first time which had a Cloud based and Desktop client available.

The schematic has the male and female sata connectors connected pin to pin, except for the 3.3v line which is switched either pin to pin or to the 3.3v regulator output.

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/schematic.png">

## Fabrication
For the PCB I have been using JLCPCB who have been very reliable and accurate when producing my PCB designs.

I have also used their PCBA process a few times now, so I thought they could assemble the pcb's for this project as well.

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/images/pcb-top.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/images/pcb-bottom.png" width="300"> 
<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/images/3D_PCB1_2025-02-07-top.png" width="300">

## Testing
Adaptor board worked out of the box and it made easy work for both reading and writing sata drives.

## Issues
During the ordering process, it became apparent that both sata connectors were not available from JLCPCB parts stock, so I had to use their parts ordering process. I had never used that process before but the support was excellent and getting the parts didn't take long at all. Only a few days.

When the pcb was being assembled there was also an issue placing the male sata connector (J1). There were some dimensional issues with the footprint so the manufacturing team had to use some persuation in placing the component. This did not effect the soldering or function of the component. Todo - modify pcb footprint for future designs.

When routing the PCB, the GND traces on either side of the Data traces had Vias so that they were stitched to the bottom PCB ground fill. I did not define them correctly before placing so they were effectivley isolated from the ground plane. I have fixed that issue in version 1.1.

## Manufacturing Files
todo
