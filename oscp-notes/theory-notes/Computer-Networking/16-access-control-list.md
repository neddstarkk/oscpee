# 16. Access Control List

## Packet Filtering

* Used to allow or deny traffic
  * Also used for NAT, QoS, etc.
* Defined on the ingress or egress of an interface
  * Incoming or outgoing
* ACLs can evaluate on certain criteria
  * Source IP, destination IP, TCP port numbers, UDP port numbers, ICMP
* Deny or permit
  * What happens when ACL matches the traffic?
* ACLs have evolved through the years
  * More options and features available for traffic filtering

## Firewall rules

* Access Control Lists (ACLs)
  * Allow or disallow traffic based on tuples
  * Groupings of categories
    * Source IP, Destination IP, port number, time of day, application, etc.
  * A logical path
    * Usually top-to-bottom
  * Can be very general or very specific
    * Specific rules are usually at the top
  * Implicit deny
    * Most firewalls include a deny at the bottom
      * Even if you didn't put one

## Web server firewall ruleset

| Rule Number | Remote IP | Remote Port | Local Port | Protocol | Action |
|:-----------:|:---------:|:-----------:|:----------:|----------|--------|
|      1      |    All    |     Any     |     22     |    TCP   |  Allow |
|      2      |    All    |     Any     |     80     |    TCP   |  Allow |
|      3      |    All    |     Any     |     443    |    TCP   |  Allow |
|      4      |    All    |     Any     |    3389    |    TCP   |  Allow |
|      5      |    All    |      53     |     Any    |    UDP   |  Allow |
|      6      |    All    |     123     |     Any    |    UDP   | Allow  |
|      7      |    All    |             |            |    ICMP  | Deny   |
