# 11. Static and Dynamic Routing

## Routing

* Send IP packets across the network
  * Forwarding decisions based on destination IP address
* Each router only knows the next step

## Static Routing

* Administratively define the routes
  * You are in control
* Advantages
  * Easy to configure and manage on smaller networks
  * No overhead from routing protocols(CPU, memory, bandwidth)
  * Easy to configure on sub networks (only one way out)
  * More secure - no routing protocols to analyze
* Disadvantages
  * Difficult to administer
  * No automatic method to prevent routing loops
  * If there's a network change, you have to manually update the routes
  * No automatic rerouting if an outage occurs

## Dynamic Routing

* Routers send routes to other routers
  * Routing tables are updated in (almost) real-time
* Advantages
  * No manual route calculations or management
  * New routes are populated automatically
  * Very scalable
* Disadvantages
  * Some router overhead required (CPU, memory, bandwidth)
  * Requires some initial configuration to work properly

## Default Route

* A route when no other route matches
  * A "gateway of last resort"
* A remote site may have only one route
  * Go that way -> rest of the world
* Can dramatically simplify the routing process
  * Works in conjunction with all other routing methods
