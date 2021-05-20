# IPv4 and IPv6 addressing

## The IP address of a device

* IP address, e.g. 192.168.1.165
  * Every device needs a unique IP address
* Subnet Mask, e.g. 255.255.255.0
  * Used by the local workstation to determine what subnet it's on
    * The subnet mask (usually) isn't transmitted across the network
    * You'll ask for the subnet mask all the time
      * What's the subnet mask of this network?

## The secret behind the IP address

* The IP address isn't really a single address
* An IP address is a combination of a network ID and a host ID
  * The subnet mask determines what part of the IP address is the network and which part is the host
    * The subnet mask is just as important as your IP address!
* The best way to see this work is in binary
  * This is the very easy math part that I already know so I am gonna skip

## IPv4

* Internet Protocol version 4
* OSI layer 3
* Since one byte is 8 bits, the maximum decimal value for each byte is 255

## IPv6

* Internet protocol version 6
* 128 bit address
* 340 undecillion addresses
* Your DNS becomes very important!

## IPv6 address compression

* Groups of zeroes can be abbreviated with a double colon
  * Only one of these abbreviations allowed per address
* Leading zeroes are optional

2600:DDDD:1111:0001:0000:0000:0000:0001

Remove leading zeroes

2600:DDDD:1111: 1:  0:  0:  0:  1

Abbreviate 2+ groups of zeroes with double colons

2600:DDDD:1111::1
