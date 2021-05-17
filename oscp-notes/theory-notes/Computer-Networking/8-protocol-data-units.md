# 8. Protocol Data Units

## PDU (Protocol Data Unit)

* A unit of transmission
  * A different group of data at different OSI layers
* Ethernet operates on a frame of data
  * it has no idea what's inside
* IP operates on a packet of data
  * Inside is TCP or UDP, but it doesn't know that
* TCP or UDP PDU
  * TCP segment
  * UDP segment

## Maximum Transmission Unit (MTU)

* Maximum IP packet to transmit
  * but not fragment
* Fragmentation slows things down
  * Losing a fragment means losing an entire packet
  * Requires overhead along the path
* Difficult to know the MTU all the way through the path
  * Automated methods are often inaccurate
    * Especially when ICMP is filtered

## Troubleshooting MTU

* MTU sizes are usually configured once
  * Based on the network infrastructure and don't change often
* A significant concern for tunneled traffic
  * The tunnel may be smaller than your local ethernet segment
* What if you send packets with Don't Fragment(DF) set?
  * Routers will respond back and tell you to fragment
  * Hope you get the ICMP message!
* Troubleshoot using ping
  * ping with DF and force a maximum size of 1472 bytes
  * 1500 bytes - 8 byte ICMP header - 20 bytes IP address = 1472
    * Windows: ping -f -l 1472 8.8.8.8
