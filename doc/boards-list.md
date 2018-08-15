Boards list and Pin connection to Arduino-LMIC library
====================

The objetcive of this documment is to provide an easy tool to select the correct pin mapping to connect diferrent boards with the LMIC library.

### SX1276 MBED Shield

The [SX1276 Mbed shield](https://os.mbed.com/components/SX1276MB1xAS/) is built based on the SX1276 transceiver which, added to a high-performance FSK / OOK RF transceiver modem, features the LoRa™ long range modem.

For this borad the pin mapping could look like this:

	lmic_pinmap lmic_pins = {
	    .nss = 10,
	    .rxtx = LMIC_UNUSED_PIN,
	    .rst = A0,
	    .dio = {2, 3, 4},
	};
  
### LoRa Node - Whisper Board
LoRa node, from [Wisen](https://wisen.com.au/store/products/whisper-node-lora/) is a real ultra-low power LoRa development board based on the popular Atmel AVR ATMega328p - Arduino compatible.

For this borad the pin mapping could look like this:

	lmic_pinmap lmic_pins = {
	    .nss = 10,
	    .rxtx = LMIC_UNUSED_PIN,
	    .rst = 7,
	    .dio = {2, A2, A3},
	};
  
