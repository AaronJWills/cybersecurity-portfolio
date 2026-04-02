# TryHackMe : Networking Essentials

**Path:** Cyber Security 101
**Completed:** 
**Difficulty:**

## Overview
Dynamic Host Configuration Protocol (DHCP)
Address Resolution Protocol (ARP)
Network Address Translation (NAT)
Internet Control Message Protocol (ICMP)
Ping
Traceroute

## Key Skills Practised
-


## Useful Commands / Tools


## Screenshots
DHCP packet request
user@TryHackMe$ tshark -r DHCP-G5000.pcap -n
    1   0.000000      0.0.0.0 → 255.255.255.255 DHCP 342 DHCP Discover - Transaction ID 0xfb92d53f
    2   0.013904 192.168.66.1 → 192.168.66.133 DHCP 376 DHCP Offer    - Transaction ID 0xfb92d53f
    3   4.115318      0.0.0.0 → 255.255.255.255 DHCP 342 DHCP Request  - Transaction ID 0xfb92d53f
    4   4.228117 192.168.66.1 → 192.168.66.133 DHCP 376 DHCP ACK      - Transaction ID 0xfb92d53f

## Takeaway for Security Roles
DHCP is an application-level protocol that relies on UDP; the server listens on UDP port 67, and the client sends from UDP port 68
DHCP follows four steps: Discover, Offer, Request, and Acknowledge (DORA)
