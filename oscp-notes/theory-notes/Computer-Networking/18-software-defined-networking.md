# 18. Software-Defined Networking

## SDN

* Networking devices have two functional planes of operation
  * Control plane, data plane
* Control Plane is responsible for the administration and the ongoing servicing of a particular device
* Data Plane is responsible for transferring data from one point to another
* SDNs are directly programmable
  * Configuration is different than forwarding
* Agile
  * Changes can be made dynamically
* Centrally managed
  * Global view, single pane of glass
* Programmatically configured
  * Orchestration
  * No human intervention
* Open standards / vendor neutral
  * A standard interface to the network

## Distributed Switching

A lot of this SDN functionality is enabled, because we virtualized a huge portion of our infrastructure. We have servers and routers and firewalls and switches that are now in a virtual world. 

* Remove the physical segmentation
  * A virtual network distributed across all physical platforms
* When a VM moves, the network doesn't change
  * Servers will always connect to the right VLAN
