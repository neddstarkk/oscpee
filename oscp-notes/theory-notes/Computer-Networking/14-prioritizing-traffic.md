# 14. Prioritizing Traffic

## Managing Network Traffic

* Many different devices
  * Desktop, laptop, VoIP phone, mobile devices
* Many different applications
  * Mission critical applications, streaming video, streaming audio
* Different apps have different network requirements
  * Voice is real-time
  * Recorded video streaming has a buffer
  * Database application is interactive
* Some applications are "more important" than others
  * Voice traffic needs to have priority over YouTube

## Packet Shaping

* packet shaping, traffic shaping
* Control with bandwidth usage or data rates
* Set important applications to have higher priorities than other apps

## Quality of Service (QoS)

* Prioritize traffic performance
  * Voice over IP traffic has priority over web-browsing
  * Prioritize by maximum bandwidth, traffic rate, VLAN, etc.
* Quality of Service
  * Describes the process of controlling the traffic flows
* Many different methods
  * Across many different topologies

## Managing QoS

* Class of Service (CoS)
  * OSI layer 2
  * Ethernet frame header in 802.1Q trunk
  * Usually applied on the intranet (not from an ISP) since we don't have trunk connections to an ISP
* Differentiated Services (DiffServ)
  * OSI layer 3
  * QoS bits enabled in the IPv4 header
  * Bits are set external to the application
  * Routers apply the QoS
* Differentiated Services Code Point (DSCP)
  * DS (Differentiated Services) field in the IP header
