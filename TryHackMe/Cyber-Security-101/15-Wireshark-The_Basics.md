# TryHackMe : Wireshark The Basics
https://tryhackme.com/room/wiresharkthebasics

**Path:** Cyber Security 101
**Completed:** 7 April, 2026
**Difficulty:** Easy

## Overview
Learning the basics of Wireshark and how to analyse protocols and PCAP files.  

## Key Skills Practised
- Navigating and configuring Wireshark.
- Inspecting packets and info from the different TCP/IP layers.
- Using display filters

## Useful Commands / Tools
- Statistics --> Capture File Properties (shows the file details)
- File --> Merge (merge PCAP files)
- View --> Coloring Rules (create permanent colouring rules)
- Go --> Go to packet (go to a specific packet number)
- Edit --> Find Packet (searching inside packets for a particular event of interest.  You should select the type of input - Display filter, Hex, String and Regex.  You want to select which pane you're searching in as well - packet list, packet details or packet bytes)
- Edit --> Mark/Unmark packets
- Edit --> Packet comments
- File --> Export Specified Packets
- File --> Export Objects
- View --> Time Display Format
- Analyse --> Expert Information (spot anomolies and problems)
- Analyze --> Apply as Filter
- Analyze --> Conversation Filter (analyze all linked packets)
- View --> Colourise Conversation
- Analyze --> Prepare as Filter (to chain multiple queries together with and/or)
- Analyse --> Follow TCP/UDP/HTTP Stream (reconstruct the streams and view the raw traffic as it is presented at the application level)
- Filter by Protocol name - just type the protocol name (http, arp, dhcp, ftp, smtp, pop, imap, and more) into the display filter
- Filter by port - tcp.port == portnumber or udp.port == portnumber into the display filter
- Filter by IP - ip.addr == IPaddress

## Screenshots
<img width="1558" height="735" alt="image" src="https://github.com/user-attachments/assets/c1f526c0-0e94-489f-8355-97b67eb6557f" />

<img width="1200" height="460" alt="image" src="https://github.com/user-attachments/assets/acab4038-fac0-40fe-ae55-8f9669c8578f" />

<img width="1590" height="710" alt="image" src="https://github.com/user-attachments/assets/e8fb37ee-b902-4bd4-b37e-5495a3838cb0" />

## Takeaway for Security Roles
The Frame (Layer 1):This will show you what frame/packet you are looking at and details specific to the Physical layer of the OSI model.
Source [MAC] (Layer 2):This will show you the source and destination MAC Addresses; from the Data Link layer of the OSI model.
Source [IP] (Layer 3):This will show you the source and destination IPv4 Addresses; from the Network layer of the OSI model.
Protocol (Layer 4):This will show you details of the protocol used (UDP/TCP) and source and destination ports; from the Transport layer of the OSI model.
Protocol Errors:This continuation of the 4th layer shows specific segments from TCP that needed to be reassembled.
Application Protocol (Layer 5):This will show details specific to the protocol used, such as HTTP, FTP,  and SMB. From the Application layer of the OSI model. 
Application Data: This extension of the 5th layer can show the application-specific data.

Golden rule for analysts who don't want to write queries for basic tasks: "If you can click on it, you can filter and copy it"
