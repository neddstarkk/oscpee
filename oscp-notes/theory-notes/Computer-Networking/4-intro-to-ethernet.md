# 4. Introduction to Ethernet

## The Ethernet Frame

|**Field**   |**Bytes** |**Description** |
|---|---|---|
|Preamble   |7   |56 alternating ones and zeroes used for synchronization (101010..)   |
|SFD   | 1  | Start Frame Delimiter - designates the end of the preamble (10101011)  |
|Destination MAC address   | 6  | Ethernet MAC address of the destination device  |
|Source MAC address   | 6  | Ethernet MAC address of the source device  |
|Ether Type   | 2  |Describes the data contained in the payload   |
|Payload | 46 - 1500 | Layer 3 and higher data |
|FCS | 4 | Frame Check Sequence - CRC checksum of the frame |

## The MAC address

* Ethernet Media Access Control address
  * The "physical" address of a network adapter
  * Unique to a device
* 48 bits / 6 bytes long
  * Displayed in hexadecimal
  * The first three bytes are Organizationally Unique Identifier (OUI) of the manufacturer.
  * Last three bytes are Network Interface Controller Specific bytes (the serial number)

## Duplex

* Half-duplex
  * A device cannot send and receive simultaneously
  * All LAN hubs are half-duplex devices
  * Switch interfaces can be configured as half-duplex
    * But usually only when connecting to other half-duplex device
* Full-duplex
  * Data can be sent and received at the same time
  * A properly configured switch interface will be set to full duplex.

## Half duplex ethernet

* Traffic received on one interface is repeated to all other interfaces
* If two devices communicate simultaneously, you have a collision

## CSMA/CD

* CS - Carrier Sense
  * Is there a carrier?
  * Is there a signal available that we can use to send some data?
* MA - Multiple Access
  * More than one device on the network
* CD - Collision Detect
  * Collission - Two stations talking at once
  * Identify when data gets garbled
* Half duplex ethernet
  * not used any longer.

## Full duplex ethernet

* Full duplex
  * Send and receive simultaneously

## CSMA/CA

* CA - Collision Avoidance
  * Common on wireless networks
* Collision Detection isn't possible
  * A sending station can't "hear" other stations
* Use RTS/CTS
  * I am Ready to send
  * You are Clear to send
* Solves the "hidden node" problem
  * Station A can hear the access point
  * Station B can hear the access point
  * Station A can't hear Station B
