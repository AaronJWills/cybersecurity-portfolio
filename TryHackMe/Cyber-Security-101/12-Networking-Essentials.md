# TryHackMe : Networking Essentials

**Path:** Cyber Security 101
**Completed:** 2 April, 2026
**Difficulty:** Easy

## Overview
- Dynamic Host Configuration Protocol (DHCP)
- Address Resolution Protocol (ARP)
- Network Address Translation (NAT)
- Internet Control Message Protocol (ICMP)

## Key Skills Practised

## Useful Commands / Tools
ICMP - 'ping', 'tracert' (windows) 'traceroute' (Linux)

## Screenshots
DHCP packet request

<img width="668" height="98" alt="image" src="https://github.com/user-attachments/assets/8677c1b6-37ab-4685-bafe-9655e7e144d4" />

ARP in action

<img width="932" height="253" alt="image" src="https://github.com/user-attachments/assets/8a1d4321-2dcc-468e-9ecb-a4c742ea003b" />

NAT enabled router contains tables for internal and external IPs and ports

<img width="695" height="538" alt="image" src="https://github.com/user-attachments/assets/e4fc5211-ad43-4ba4-9a48-94d1d36a0b01" />


## Takeaway for Security Roles
DHCP is an application-level protocol that relies on UDP; the server listens on UDP port 67, and the client sends from UDP port 68
DHCP follows four steps: Discover, Offer, Request, and Acknowledge (DORA)
Routing protocols 
- OSPF (Open Shortest Path First): OSPF is a routing protocol that allows routers to share information about the network topology and calculate the most efficient paths for data transmission.
- EIGRP (Enhanced Interior Gateway Routing Protocol): EIGRP is a Cisco proprietary routing protocol that combines aspects of different routing algorithms.
- BGP (Border Gateway Protocol): BGP is the primary routing protocol used on the Internet.
- RIP (Routing Information Protocol): RIP is a simple routing protocol often used in small networks.
NAT - the number of IP addresses is always expressed as a power of two. You reserve two public IP addresses instead of thirty-two. Consequently, you would have saved thirty public IP addresses.
