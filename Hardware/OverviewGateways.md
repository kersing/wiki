# Introduction
On the gateway side there's a few options. 
The Gateway has a communication part and a calculation part. 
The gateway supports many nodes thus the calculation part should be bigger
than the node.

For **Communication** there are two options for the chip the SX1272/SX1276 option and the SX1301 + SX1257 option.
*the SX1272/SX1276 only allows for one (1) connection at a time,
*the SX1301 + SX1257 chips allows up to eight (8() simultaneous connections (typically supporting 10000 ~ 20000 nodes).
For the **Calculation** part a device that supports linux is usually used. These are provided by many many suppliers, more on this in ouw Hardware Gateway Overview.

At the moment there are several options to get you own gateway. These fall into two categories:
* Ready to roll
* Do it yourself

There is also a third option, that is design your own hardware,
but that is beyond the scope of this how-to.

## Ready to roll
Depending on how much money you want to spend and when the hardware is needed the following options are available (from most expensive to least expensive):

### [The Things Gateway](http://thethingsnetwork.org/kickstarter-landing/kickstarter.html)
* Price: 200 euro 
* Availability: [the kickstarter](http://kickstarter.com/projects/419277966/the-things-network) runs until Fri, Nov 20 2015 1:44 PM CET!
* Capacity: 8 band, ~ 20K Nodes 
* Suitable for indoor use
* Installation: Plug and play
* Hardware: open source 
* Software: open source
Tested by The Things Network Crew.
Discussion: The device is specially developed for The Things Network and we will make sure it will meet all requirements for a smooth experience on The Things Network. Note that estimated first delivery is around June 2016.

### [Kerlink](http://www.kerlink.fr/en/)
* Price: on request, around 1.200 euro / 1.500 dollar.
* Availability: direct available, send inquiry to [Kerlink Sales](mailto:sales@kerlink.fr)
* Capacity: 8 band, ~ 20K Nodes 
* Suitable for outdoor mounting (IP67)
* Installation: requires a technician
* Hardware: proprietary
* Software: open source & proprietary
* Possibility to run on gprs/3g network
* Tested by The Things Network Crew.
* Manual: [Installation guide](/wiki/Installing-your-Kerlink)

Discussion: This is an industrial solution suitable for people who want to mount the gateway outside and have sufficient technical skills to connect, mount and maintain the device themselves. We have tested the device and although we have remarks about the somewhat older software that is being used, this device will do the job. A trained software engineer will be able to update the device using the software from The Things Network. 


### [MultiTech](http://www.multitech.com/brands/multiconnect-conduit)
* Price: on request, around 700 euro, may require additional boards to run
* Availability: unknown
* Capacity: ? 
* Suitable for indoor use
* Installation: Plug and play (?)
* Hardware: proprietary
* Software: proprietary (?)
* Tested by The Things Network Crew. 

Discussion: We have one, results of our test will follow asap. 
First draft of an [installation guide](/wiki/Installing-your-Multitech-mLinux-Conduit)

### [Lorank 8](http://www.hoperf.nl/LORANK-8)
* Price: 412 euro 
* Availability: pre-order, estimated delivery time 30 days
* Capacity: 8 band, ~ 20K Nodes 
* Suitable for indoor use
* Installation: Plug and play
* Hardware: radio proprietary, MCU board: open source 
* Software: open source
* Tested by The Things Network Crew.

Discussion: The device is build upon the radio board of IMST and the open
source hardware BeagleBone Black. Although the first version had some
issues, at this moment the device seems to work as advertised. Please consult
the online manual for further information.

### [LinkLabs 868 MHz LoRaWAN Gateway with Wifi](http://store.link-labs.com/products/868-mhz-lorawan-gateway-with-wifi)
* Price: 633 euro ($697) (promotion at 360 euro ($397) ended March 1'st )
* Availability: ships in 6-8 weeks
* Capacity: 8 band 
* Suitable for indoor use
* Installation: Plug and play
* Hardware: proprietary 
* Model: unknown (LL-BST-8-868?)
* Software: proprietary
* Includes: GPS (Class B ready) Antenna
* Not yet tested by The Things Network Crew?

### [IMST IC880a + Raspberry Pi](http://webshop.imst.de/radio-modules/lora-concentrators.html)
* Price: ~260 euro (189 euro p/board + Antenna + Pigtail + RPi + Power supply + taxes)
* Availability: In Stock.
* Capacity: 8 band, ~ 20K Nodes 
* Suitable for indoor use
* Installation: Requires a technician
* Hardware: radio proprietary, MCU board: open source 
* Software: open source
* Tested by several TTN communities.
* Installation: [Automated](https://github.com/ttn-zh/ic880a-gateway/wiki)

Basically the same as the Lorank8, but slightly more DIY.
The device is built upon the radio board of IMST and a Raspberry Pi


## Other resources
We love this comparison matrix from Loriot:
[https://www.loriot.io/lora-gateways.html](https://www.loriot.io/lora-gateways.html)

## Do it yourself
Here's other people building their own gateway:

### DIY "Real" gateway (SX1301 + SX1257)
* [https://github.com/mirakonta/lora_gateway/wiki](https://github.com/mirakonta/lora_gateway/wiki)
* [description and manual for preparing for outside use](http://www.meiland.nl/2015/12/outdoor-lora-gateway/)

### DIY "single-channel" gateway (SX1272, SX1276 etc)
* [TTN-compatible semi-LoRaWAN @tftelkamp HopeRF RFM92W/RFM95W](https://github.com/tftelkamp/single_chan_pkt_fwd) and forked with [NiceRF LoRa1276 support](https://github.com/4refr0nt/single_chan_pkt_fwd)
* [DIY lora gateway](http://cpham.perso.univ-pau.fr/LORA/RPIgateway.html) (not LoRaWAN/TTN compatible)
* [http://www.daveakerman.com/?p=1719](http://www.daveakerman.com/?p=1719) (not LoRaWAN/TTN compatible)


## Antennas

See the [Antennas](/wiki/Antennas) page.

## Network
Once you've got a gateway ready to transmit and/or receive data,
start with our **[Software Overview](/wiki/Software/Overview)**.


**[back to GettingStarted](../GettingStarted)**
