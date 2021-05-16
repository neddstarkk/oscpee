# 6. Broadcast Domains and Collision Domains

## Collision Domains

* A historical footnote
  * It's difficult to find a collision these days
  * The word "collision" is misleading
  * When driving a car, you never want a collision to occur. But on a half-duplex network, it is completely expected that collisions will occur during normal operation
* The network was one big segment
  * Everyone heard everyone else's signals
  * One big conference call
* Only one station can "talk" at a time
  * Is the line clear? Ok, I can talk
  * Carrier Sense Multiple Access (CSMA)
* When two people spoke at the same time, there was a collision
  * Collision Detection (CD)
  * Send the jam signal

## Broadcast Domains

* Spread the word
  * Everyone must know
    * ARP requests
    * Operating System notifications
    * Some dynamic routing protocols
* How far can a broadcast go?
  * Passed by switch/bridge
  * Stops at the router
* This can be important
  * More devices, more broadcasts
