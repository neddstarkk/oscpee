# 15. Network Address Translation

* It is estimated that there are over 20 billion devices connected to the internet (and growing)
  * IPv4 supports around 4.29 billion addresses
* The address space for IPv4 is exhausted
  * There are no available addresses to assign
* How does it all work?
  * Network Address Translation

## NAT overload / PAT / Source NAT

* Source NAT - cos we're performing NAT on the source IP
* PAT - Port Address Translation

## Port Forwarding

* 24x7 access to a service hosted internally
  * Web server, gaming server, security system, etc.
* External IP/port number maps to an internal IP/port
  * Does not have to be the same port number
* Also called Destination NAT or static NAT
  * Destination address is translated from a public IP to a private IP
  * Does not expire or timeout