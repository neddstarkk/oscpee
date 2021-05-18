# 12. IGP and EGP

## AS (Autonomous System)

* Autonomous
  * Existing as an independent entity
* Group of IP routes under common control
* RFC 1930, Section 3: Definitions
  * "An AS is a connected group of one or more IP prefixes run by one or more network operators which has a SINGLE and CLEARLY DEFINED routing policy."
* Important point of reference for discussing Interior Gateway Protocol and Exterior Gateway Protocols

## IGP (Interior Gateway Protocol)

* Used within a single autonomous system (AS)
  * Not intended to route between AS
    * That's why there's EGPs
* IPv4 dynamic routing
  * OSPFv2 (Open Shortest Path First)
  * RIPv2 (Routing Information Protcol version 2)
  * EIGRP (Enhanced Interior Gateway Routing Protocol)
* IPv6
  * OSPFv3
  * EIGRP for v6
  * RIPng (next generation)

## EGP (Exterior Gateway Protocol)

* Used to route between AS
  * Leverages the IGP at the AS to handle local routing
* BGP (Border Gateway Protocol)
  * Many organizations use BGP as their EGP

