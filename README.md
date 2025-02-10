# sata 3.3v injector

## Background
I came across these sata 16GB drives that I could not read or write to with a standard USB to SATA adaptor. (similar drive pictured below)

<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-16gb-front.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/sata-16gb-back.png" width="300"> <img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/usb-sata-cable.png" width="300"> 

Apparently both the 5v and 3.3v supplies were required to achive this. So I thought I would design my adaptor to solve this issue.

A voltage regualtor to drop the 5v rail down to 3.3v would be an easy solution.

## Design
The AMS1117-3.3 was a good choice for the regulator as it can supply up to 1Amp. Add a smoothing and noise capacitor and its done.
<img src="https://github.com/kaza007/sata-3.3v-injector/blob/main/regulator-circuit.png" width="300"> 

The sata standard...
