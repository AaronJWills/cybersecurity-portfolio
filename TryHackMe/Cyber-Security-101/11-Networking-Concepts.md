# TryHackMe : Networking Concepts
https://tryhackme.com/room/networkingconcepts

**Path:** Cyber Security 101
**Completed:** 28 March, 2025
**Difficulty:** Easy

## Overview
ISO OSI model and the TCP/IP protocol suite.

## Key Skills Practised
- Telnet


## Useful Commands / Tools
Handy acronym for remembering the OSI model -
“Please Do Not Throw Spinach Pizza Away.”

## Screenshots
Layer Number	Layer Name	Main Function	Example Protocols and Standards
Layer 7	Application layer	Providing services and interfaces to applications	HTTP, FTP, DNS, POP3, SMTP, IMAP
Layer 6	Presentation layer	Data encoding, encryption, and compression	Unicode, MIME, JPEG, PNG, MPEG
Layer 5	Session layer	Establishing, maintaining, and synchronising sessions	NFS, RPC
Layer 4	Transport layer	End-to-end communication and data segmentation	UDP, TCP
Layer 3	Network layer	Logical addressing and routing between networks	IP, ICMP, IPSec
Layer 2	Data link layer	Reliable data transfer between adjacent nodes	Ethernet (802.3), WiFi (802.11)
Layer 1	Physical layer	Physical data transmission media	Electrical, optical, and wireless signals


Layer Number	ISO OSI Model	TCP/IP Model (RFC 1122)	Protocols
7	Application Layer	Application Layer	HTTP, HTTPS, FTP, POP3, SMTP, IMAP, Telnet, SSH,
6	Presentation Layer		
5	Session Layer		
4	Transport Layer	Transport Layer	TCP, UDP
3	Network Layer	Internet Layer	IP, ICMP, IPSec
2	Data Link Layer	Link Layer	Ethernet 802.3, WiFi 802.11
1	Physical Layer		



## Takeaway for Security Roles
Private IP ranges
10.0.0.0 - 10.255.255.255 (10/8)
172.16.0.0 - 172.31.255.255 (172.16/12)
192.168.0.0 - 192.168.255.255 (192.168/16)

TCP 3 way handshake
SYN - client to server
SYN-ACK - server to client
ACK - client to server
Ports 1 to 65535

We start with the application data. 
At the transport layer, we add a TCP or UDP header to create a TCP segment or UDP datagram. 
Again at the network layer, we add the proper IP header to get an IP packet that can be routed over the internet. 
Finally we add the appropriate header and trailer to get a WiFi or Ethernet frame at the link layer.
