# 5. Network Switching

## The Switch

* Forward or drop frames
  * Based on the destination MAC address
* Gather a constantly updating list of MAC addresses
  * Builds the list based on the source MAC address of incoming traffic
* Maintain a loop-free environment
  * Using Spanning Tree Protocol(STP)

## Learning the MACs

* Switches examine incoming traffic
  * Make a note of the source MAC address
* Adds unknown MAC address to the MAC address table
  * Sets the output interface to the received interface

## Flooding for unknown MACs

* The switch doesn't always have a MAC address in the table
* When in doubt, send the frame to everyone

## Address Resolution Protocol

* Determine a MAC address based on an IP address
  * You need a hardware address to communicate
