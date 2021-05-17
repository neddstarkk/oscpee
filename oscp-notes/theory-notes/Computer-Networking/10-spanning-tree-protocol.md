# 10. Spanning Tree Protocol

## Loop Protection

* Connect two switches to each other
  * Create a loop with two cables
  * They'll send traffic back and forth forever
  * There's no "counting" mechanism at the MAC layer
* This is an easy way to bring down a network
  * And somewhat difficult to troubleshoot
  * Relatively easy to resolve
* IEEE standard 802.1D to prevent loops in bridged (switched) networks (1990)
  * Created by Radia Perlman
  * Used practically everywhere

## STP port states

* Blocking
  * Not forwarding to prevent a loop
* Listening
  * Not forwarding and cleaning the MAC table
* Learning
  * Not forwarding and adding to the MAC table
* Forwarding
  * Data passes through and is fully operational
* Disabled
  * Administrator has turned off the port

## Rapid Spanning Tree Protocol (RSTP/802.1w)

* A much needed update of STP
* This is the latest standard
* Faster convergence
  * from 30 to 50 seconds to 6 seconds
* Backwards compatible with 802.1D STP
  * You can mix both in your network
* Very similar process
  * an update, not a wholesale change
