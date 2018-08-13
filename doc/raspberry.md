# Raspberry Pi Set up to LoRaWAN gateway

Please follow the steps listed below:

1) Download [Raspbian Stretch Lite](https://www.raspberrypi.org/downloads/raspbian/)
2) Follow the [installation guide](https://www.raspberrypi.org/documentation/installation/installing-images/README.md) to create the SD card
3) [Enable one-time SSH](https://www.raspberrypi.org/blog/a-security-update-for-raspbian-pixel/)
4) Use `sudo raspi-config` utility to

        $ sudo raspi-config

    - **Enable SPI** (`5 Interfacing Options -> P4 SPI`)
    - **Enable SSH** (`5 Interfacing Options -> P2 SSH`)
    - Set hostname (`2 Network Options -> N1 Hostname`)
    - Change locale (`4 Localisation Options -> I1 Change Locale`)
    - Change timezone (`4 Localisation Options -> I2 Change Timezone`)
    
5) Make sure that you are on the latest version of the Raspbian image, and install Git: 

        $ sudo apt-get update
        $ sudo apt-get upgrade
        $ sudo apt-get install git

Ok, once you have done these steps the Raspberry Pi basic image is good to go to next steps...

