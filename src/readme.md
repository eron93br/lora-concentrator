## Arduino-LMIC library (AU915 version)

This repository contains the IBM LMIC (LoraMAC-in-C) library, slightly modified to run in the Arduino environment, allowing using the SX1272, SX1276 tranceivers and compatible modules (such as some HopeRF RFM9x modules).

This library mostly exposes the functions defined by LMIC, it makes no attempt to wrap them in a higher level API that is more in the Arduino style. To find out how to use the library itself, see the examples, or see the PDF file in the doc subdirectory.

This library requires Arduino IDE version 1.6.6 or above, since it requires C99 mode to be enabled by default.

The main changes were done in the [lorabase.h](https://github.com/eron93br/lora-concentrator/blob/master/src/lmic/lorabase.h) file.

License
-------
Most source files in this repository are made available under the
Eclipse Public License v1.0. The examples which use a more liberal
license. Some of the AES code is available under the LGPL. Refer to each
individual source file for more details.
