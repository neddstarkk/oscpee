# Network Segmentation

## LANs

* A group of devices in the same broadcast domain
* Difficult to scale when thousands of different devices come into play

## Virtual LANs

* Virtual Local Area Networks
  * A group of devices in the same broadcast domain
  * Separated logically inside the switch instead of physically

How to configure VLAN on multiple switches?
One way to do this would be to run a separate cable for VLAN 1 and separate cable for VLAN 2. However this would not scale very well once you have a larger number of VLANs. What if there are 100 VLANs on a switch, or a 1000? You wouldn't even have enough interfaces on the switch to connect them.

Instead you would create what's called a trunk. This trunk connection is a single physical connection between those switches but it's able to transmit multiple VLANs across that connection.

## IEEE 802.1Q Trunking

* Take a normal ethernet frame
* Add a VLAN header in the frame
* VLAN IDs - 12 bits long, 4094 VLANs
  * "Normal Range" - 1 through 1005, "Extended Range" - 1006 through 4094
  * 0 and 4095 are reserved VLAN numbers
