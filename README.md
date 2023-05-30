# corolla-can
Investigations into CAN-bus traffic on 2015 Toyota Corolla 


This repo contains documentation of my investigating CAN traffic on a vehicle. By taking packet captures of the CAN bus during controlled experiments, I hope to enumerate the sensor traffic and gain insight into the Controller Area Network

# Hardware: 
InnoMaker USB2CAN adapter (https://github.com/INNO-MAKER/usb2can)

# Software:
Manufacturer-provided proof-of-concept software. Planning to implement C/C++/Python soon. 

# Notes: 
--> Baud rate is 500k 

--> More needs to be written about the "polling" observed in the network. Before any node on the network transmits its updated value, a specific sequence of frames are transmitted from 0x440 and 0x442. They are      identical in almost all of my observations. 

--> So far I have not been able to spoof traffic on the network. 
