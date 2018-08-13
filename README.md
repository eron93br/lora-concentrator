# LoRaWAN gateway based on LoRa concentrator

This document describes the basic setup of the LoRaWAN gateway based either on the iC980a module or RAK831 module. 
The objective is to build a LoRaWAN multichannel gateway based on the SEMTECH Packet Forwarder implementation.

Gateway Features
--------
- Listen on configurable frequency and spreading factor
- Support to all spreading factors (SF7 to SF12)
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
- The Things Network gateway registration 

Setup based on Raspbian image
--------
Follow these instructions

Regulations
--------
- [LoRaWAN Frequency Plans and Regulations by Country](https://www.thethingsnetwork.org/docs/lorawan/frequencies-by-country.html)
- [The Things Network Fair Access Policy](https://www.thethingsnetwork.org/forum/t/limitations-data-rate-packet-size-30-seconds-uplink-and-10-messages-downlink-per-day-fair-access-policy/1300)

LICENSE
--------
to-do
