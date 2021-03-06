# LoRaWAN gateway based on LoRa concentrator

This document describes the basic setup of the LoRaWAN gateway based either on the iC980a module or RAK831 module. 
The objective is to build a LoRaWAN multichannel gateway based on the SEMTECH Packet Forwarder implementation.

Gateway Features
--------
- Listen on configurable frequency and spreading factor
- Supporting Spreading Factors SF7 to SF10 
- Uplink and downlink messages

Hardware components 
--------
- Raspberry Pi 3 (not tested yet  on the Raspberry Pi Zero or Pi Zero W)
- LoRa concentrator module: either RAK831 or iC980/iC880a
- 868/915 MHz antenna
- Connection board (to connect RAK831 or iC980 to the Raspberry Pi)
- Jumpers/wires

Software setup
--------
- Raspbian Lite image on the SD Card
- Lora Gateway and Packet Forwarder installation 
- The Things Network gateway registration 

Setup based on Raspbian image
--------
Follow [these](https://github.com/eron93br/lora-concentrator/blob/master/doc/raspberry.md) instructions to create your SD card image, then install [SEMTECH](https://github.com/eron93br/lora-concentrator/blob/master/doc/software.md) packages. Set up your hardware following [this](https://github.com/eron93br/lora-concentrator/blob/master/doc/pin-connection.md) pin connection and finally [register](https://www.thethingsnetwork.org/docs/gateways/registration.html) your gateway at TTN!

Regulations
--------
- [LoRaWAN Frequency Plans and Regulations by Country](https://www.thethingsnetwork.org/docs/lorawan/frequencies-by-country.html)
- [The Things Network Fair Access Policy](https://www.thethingsnetwork.org/forum/t/limitations-data-rate-packet-size-30-seconds-uplink-and-10-messages-downlink-per-day-fair-access-policy/1300)

LICENSE
--------
The source files in this repository are made available under the following licenses:
- LoRa packet forwarder and LoRa gateway are available under [this license](https://github.com/Lora-net/lora_gateway/blob/master/LICENSE).
- The edited LMIC library is available under the Eclipse Public License v1.0.

Eclipse Public License v1.0, except for the base64 implementation, that has been copied from the Semtech Packet Forwader.
