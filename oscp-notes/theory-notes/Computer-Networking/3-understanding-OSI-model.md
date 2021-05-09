# 3. Understanding OSI Model

## The OSI Model

What is the OSI model?
Open Systems Interconnection reference model

## Layer 1 - Physical Layer

* The physics of the network
  * signaling, cabling, connectors
  * This layer isn't about protocols
* "You have a physical layer problem"
  * Fix your cabling, punch-downs, etc.
  * Run loopback tests, test/replace cables, swap adapter cards

## Layer 2 - Data Link Layer

* The basic network "language"
  * The foundation of communication at the data link layer
* Data Link Control (DLC) protocols
  * MAC (Media Access Control) address on the ethernet
* The "switching" layer

## Layer 3 - Network Layer

* The "routing" layer
* Internet Protocol (IP)
* Fragments frames to traverse different networks

## Layer 4 - Transport Layer

* The "post office" layer
  * Parcels and letters
* Transmission Control Protocol (TCP) and User Datagram Protocol (UDP)

## Layer 5 - Session Layer

* Communication management between devices
  * start, stop, restart
* Control protocols, tunneling protocols

## Layer 6 - Presentation Layer

* Character encoding
* Application encryption
* Often combined with application layer

## Layer 7 - Application Layer

* The layer we see
* HTTP, FTP, DNS, POP3
