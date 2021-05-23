# 19. Classful Subnetting

* Very specific subnetting architecture
  * Not used since 1993
    * But still referenced in casual conversation
* Used as a starting point when subnetting
  * Standard values

## The construction of a subnet

* Network address
  * The first IP address of a subnet
  * Set all host bits to 0 (0 decimal)
* First usable host address
  * One number higher than the network address
* Network broadcast address
  * The last IP address of a subnet
  * Set all host bits to 1 (255 decimal)
* Last usable host address
  * one number lower than broadcast address

## Subnet calculations

* IP address: 10.74.222.11
  * Class A
  * Subnet mask 255.0.0.0

|                                           | Network  | Host         |
|-------------------------------------------|----------|--------------|
|                                           |10.       |74. 222. 11   |
|Network address (set all host bits to 0)   |10.       |0. 0. 0       |
|First host address (add one)               |10.       |0. 0. 1       |
|Broadcast address (Set all host bits to 1) |10.       |255. 255. 255 |
|Last host address (subtract one)           |10.       |255. 255. 254 |


