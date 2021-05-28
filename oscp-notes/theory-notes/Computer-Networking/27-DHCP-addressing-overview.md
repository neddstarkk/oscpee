# 27. DHCP Addressing overview

## DHCP

* IPv4 address configuration used to be manual
  * IP address, subnet mask, gateway, DNS servers, NTP servers, etc.
* October 1993 - The bootstrap protocol
  * BOOTP
* BOOTP didn't automatically define everything
  * Some manual configurations were still required
  * BOOTP also didn't know when an IP address might be available again
* Dynamic Host Configuration Protocol
  * Initially released in 1997, updated through the years.
  * Provides automatic address / IP configuration for almost all devices

Step 1: Discover
Step 2: Offer
Step 3: Request
Step 4: Acknowledgement

## Managing DHCP in the enterprise

* Limited communication range
  * Use the IPv4 broadcast domain
  * Stops at a router
* Multiple servers needed for redundancy
  * Across different locations
* Scalability is always an issue
  * May not want (or need) to manage DHCP servers at every remote location
* You're going to need a little help(er)
  * Send DHCP request across broadcast domains
