# 1. Introduction To IP

* Efficiently move large amounts of data
  * use a shipping truck

* The network topology is the road
  * Ethernet, Cable System, DSL
  
* The truck is the Internet Protocol (IP)
  * We've designed the roads for this truck

* Inside the truck, there are boxes. The boxes hold your data
  * Boxes of TCP and UDP

* Inside the boxes are more things. So they're categorized as master bedroom, living area etc
  * Application Specific Information


## TCP and UDP

* Transported inside IP
  * Encapsulated by the IP protocol

* Two ways to move data from place to place
  * Different features for different applications. 

* OSI Layer 4
  * The transport layer

* Multiplexing
  * Use many different applications at the same time
  * TCP and UDP

### TCP - Transmission Control Protocol

* Connection-Oriented
  * A formal connection setup and close

* "Reliable" delivery
  * Recover from errors
  * Can manage out-of-order messages or transmissions.

* Flow control
  * The receiver can manage how much data is sent

### UDP - User Datagram Protocol

* Connectionless
  * No formal open or close to the connection

* "Unreliable" delivery
  * No error recovery
  * No reordering of data or retransmissions

* No flow control
  * Sender determines the amount of data transmitted.


## Speedy Delivery

* The IP delivery truck delivers from one IP address to another IP address
  * Every house has an address, every computer has an IP address

* Boxes arrive at the house / IP address
  * Where do the boxes go?
  * Each box has a room name

* Port is written on the outside of the box
  * Drop the box into the right room

## Lots of ports

* IPv4 sockets
  * Server IP address, protocol, server application port number
  * Client IP address, protocol, client port number
  
* Non-ephemeral ports - permanent port numbers
  * Ports 0 through 1023
  * Usually on a server or a service
  
* Ephemeral ports - temporary port numbers
  * Ports 1024 through 65,535
  * Determined in real-time by the client
  
* TCP and UDP ports can be any number between 0 and 65,535
* Most Servers (services) use non-ephemeral (permanent) port numbers
  * This isn't always the case. It's just a number

* Port numbers are for communication, not security
* Service port numbers need to be "well known".
* TCP port numbers aren't the same as UDP port numbers.
  * One app could be using TCP port 80, while another could be using UDP port 80. They aren't the same. 


## ICMP

* Internet Control Message Protocol
  * "Text messaging for network devices"
* Another protocol carried by IP
  * Not used for data transfer
* Devices can request and reply to administrative requests
  * Hey, are you there? Yes, I'm right here
* Devices can send messages when things don't go well
  * The network you're trying to reach is not reachable from here
  * Your time-to-live expired, just letting you know
