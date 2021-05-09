# 2. Common Ports

## Telnet

* Telnet - Telecommunication Network
  * tcp/23
* Login to devices remotely
* Console access
* In-the-clear communication (no encryption)
* Not the best choice for production systems

## SSH

* Encrypted communication link - tcp/22
* Looks and acts the same as telnet

## DNS - Domain Name System

* Converts names to IP addresses - udp/53
* These are very critical resources
  * Usually multiple DNS servers are in production

## SMTP - Simple Mail Transfer Protocol

* Server to server email transfer
* tcp/25
* Also used to send mail from a device to a mail server
  * Commonly configured on mobile devices and email clients
* Other protocols are used for clients to receive email
  * IMAP, POP3

## SFTP - Secure FTP

* Uses the SSH File Transfer Protocol
  * tcp/22
* Provides file system functionality
  * Resuming interrupted transfers, directory listings, remote file removal.
* Encrypted communication
  * Using SSH.

## FTP - File Transfer Protocol

* FTP - File Transfer Protocol
  * tcp/20 (active mode data), tcp/21 (control)
  * Transfers files between systems
  * Authenticates with a username and password
  * Full featured functionality (list, add, delete, etc.)
* TFTP - Trivial File Transfer Protocol
  * udp/69
  * Very simple file transfer application
    * Read files and write files
  * No authentication
    * Not used on production systems
  
## DHCP - Dynamic Host Configuration Protocol

* Automated configuration of IP address, subnet mask and other options
  * udp/67, udp/68
  * Requires a DHCP server
    * Server, appliance, integrated into a SOHO router, etc.
* Dynamic / pooled
  * DHCP commonly has a pool of IP addresses configured inside of the DHCP server
  * IP addresses are assigned in real-time from the pool.
  * Each system is given a lease and must renew at set intervals.
* DHCP reservation
  * Addresses are assigned by MAC address in the DHCP server
  * Quickly manage addresses from one location.

## HTTP and HTTPS

* HyperText Transfer Protocol
  * Communication in the browser
  * And by other applications
* HTTP - tcp/80 - HyperText Transfer Protocol - Web server communication
* HTTPS - tcp/443 - Hypertext Transfer Protocol Secure - Web server communication with encryption

## SNMP - Simple Network Management Protocol

* Gather statistics from network devices.
  * udp/61
* v1 - The original
  * Structured tables
  * in-the-clear
* v2 - A good step ahead
  * Data type enhancements
  * Bulk transfers
  * Still in-the-clear
* v3 - A secure standard
  * Message Integrity
  * Authentication
  * Encryption

## RDP - Remote Desktop Protocol

* Share a desktop from a remote location over tcp/3389.
* Remote desktop services on many windows versions
* Can connect to an entire desktop or just an application
* Clients for Windows, MacOS, Linux, Unix, iPhone and many others

## NTP - Network Time Protocol

* Switches, routers, firewalls, servers, workstations
  * Every device has its own clock
  * udp/123
* Synchronizing the clocks becomes critical.
  * Log files, authentication information, outage details.
* Automatic updates
  * No flashing 12:00 lights
* Flexible - You control how clocks are updated.
* Very accurate
  * Accuracy is better than 1 millisecond on a local network

## SIP - Session Initiation Protocol

* Voice over IP (VoIP) signaling
  * tcp/5060 and tcp/5061
* Setup and manage VoIP sessions
  * Call, ring, hang up
* Extend voice communication
  * Video conferencing
  * Instant messaging
  * File transfer
  
## SMB - Server Message Block

* Protocol used by Microsoft Windows
  * File sharing, printer sharing
  * Also called CIFS (Common internet file system)
* Direct over tcp/445 (NetBIOS-less)
  * Direct SMB communication over TCP without NetBIOS transport

## POP/IMAP

* Receive emails from an email server
  * Authenticate and transfer
* POP3 - Post Office Protocol version 3
  * tcp/110
  * Basic mail transfer functionality
* IMAP4 - Internet Message Access Protocol v4
  * tcp/143
  * Includes management of email inbox from multiple clients

## LDAP / LDAPS

* LDAP (Lightweight Directory Access Protocol)
  * tcp/389
  * Store and retrieve information in a network directory
* LDAPS (Lightweight Directory Access Protocol Secure)
  * A non-standard implementation of LDAP over SSL
  * tcp/636
  
## H.323

* Voice over IP (VoIP) signaling
  * ITU Telecommunication H.32x protocol series
  * tcp/1720
* Setup and manage VoIP sessions
  * call, ring, hang up
* One of the earliest VoIP standards
  * still in use today
