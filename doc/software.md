# SEMTECH gateway software

The next step of our gateway installation is set up the SEMTECH packet forwader software on the Raspberry Pi image. 

Please follow the steps listed below (on the Raspberry Pi bash):

1) Install the SEMTECH [gateway driver](https://github.com/Lora-net/lora_gateway)

        $ sudo git clone https://github.com/Lora-net/lora_gateway
 
2) Install the SEMTECH [Packet Forwarder](https://github.com/Lora-net/packet_forwarder)

        $ sudo git clone https://github.com/Lora-net/packet_forwarder

3) Clone the Reference setup for RAK831 gateways running The Things Network installer from [Kuan-Yi Li](https://github.com/kuanyili/rak831-gateway)

        $ git clone https://github.com/kuanyili/rak831-gateway.git ~/rak831-gateway
        $ cd ~/rak831-gateway
        $ sudo ./install.sh

Note that at this step you will have to configure the settings of your gateway, such as operating frequency and standard used.

## LoRa Gateway
Driver/HAL to build a gateway using a concentrator board based on Semtech SX1301 multi-channel modem and SX1257/SX1255 RF transceivers.

## Packet Forwarder 
A LoRa packet forwarder is a program running on the host of a LoRa gateway that forwards RF packets receive by the concentrator to a server through a IP/UDP link, and emits RF packets that are sent by the server.

## RAK831-Gateway
Reference setup for iC880a/iC980A/RAK831 gateways running The Things Network
