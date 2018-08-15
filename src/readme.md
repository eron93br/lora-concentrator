## Arduino-LMIC library (AU915 version)

This repository contains the IBM LMIC (LoraMAC-in-C) library, slightly modified to run in the AU915 standard with the  Arduino environment, allowing using the SX1272, SX1276 tranceivers and compatible modules (such as some HopeRF RFM9x modules).

The main changes were done in the [lorabase.h](https://github.com/eron93br/lora-concentrator/blob/master/src/lmic/lorabase.h) file. The current implementation of this library is from [Matthijs Kooijman](https://github.com/matthijskooijman/arduino-lmic).

### Pin connections
This library can be used with different models of the SX1272 and SX1276 LoRa transceiver. Using your Arduino-like board you can change the pin mapping.

For example, this could look like this:

	lmic_pinmap lmic_pins = {
	    .nss = 6,
	    .rxtx = LMIC_UNUSED_PIN,
	    .rst = 5,
	    .dio = {2, 3, 4},
	};
  
 For a specific list of boards and their pinout check out [this]() page.
 
License
-------
Most source files in this repository are made available under the Eclipse Public License v1.0. The examples which use a more liberal license. Some of the AES code is available under the LGPL. Refer to each individual source file for more details.
