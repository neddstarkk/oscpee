# 20. Assigning IPv4 addresses

## DHCP

* IPv4 address configuration used to be manual
  * IP address, subnet mask, gateway, DNS server, NTP servers, etc.
* October 1993 - The bootstrap protocol
  * BOOTP
* BOOTP didn't automatically define everything
  * Some manual configurations were still required
  * BOOTP also didn't know when an IP address might be available again
* Dynamic Host Configuration Protocol
  * Initially released in 1997, updated through the years
  * Provides automatic address / IP configuration for almost all devices

## Turning dynamic into static

* DHCP assigns an IP address from the first available from a large pool of addresses
  * Your IP address will occasionally change
* You may not want your IP address to change
  * Server, printer or personal preference
* Disable DHCP on the device
  * COnfigure the IP address information manually
  * Requires additional administration
* Configure an IP reservation on the DHCP server
  * Associate a specific MAC address with an IP address

## Automatic Private IP Addressing (APIPA)

* A link-local address
  * No forwarding by routers
* IETF has reserved 169.254.0.1 through 169.254.255.254
  * First and last 256 addresses are reserved
  * Functional block of 169.254.1.0 through 169.254.254.255
* Automatically assigned
  * Uses ARP to confirm the address isn't currently in use
