# TryHackMe : Metasploit Introduction
https://tryhackme.com/room/metasploitintro

**Path:** Cyber Security 101
**Completed:** 21 March, 2026
**Difficulty:** Moderate

## Overview
The Metasploit Framework is a set of tools that allow information gathering, scanning, exploitation, exploit development, post-exploitation, and more. While the primary usage of the Metasploit Framework focuses on the penetration testing domain, it is also useful for vulnerability research and exploit development.

Modules are small components within the Metasploit framework that are built to perform a specific task, such as exploiting a vulnerability, scanning a target, or performing a brute-force attack.
- Auxiliary-supporting modules such as scanners, crawlers & fuzzers
- Encoders-encode the exploit and payload to help signature based AV miss them
- Evasion-these modules will try to directly attempt to evade AV
- Exploits-code that uses a vulnerability
- NOPs-used as a buffer to get a consistent size payload
- Payloads-code that runs on the target system.  Types of payloads are Adapters (wraps a payload to convert it into a different format), Singles (self contained payloads), Stagers (set up connections to targets to then download the rest later), Stages (downloaded by the stager).
- Post-post-exploitation modules


## Key Skills Practised
- Learning Metasploit commands and help systems
- Launching Metasploit
- Setting options
- Running exploits
- Switching sessions

## Useful Commands / Tools
- msfconsole - launches the Metasploit console
- help
- history
- search
- use
- show options
- set
- exploit / run
- background / CTRL+Z
- sessions



## Screenshots

<img width="996" height="674" alt="Screenshot 2026-04-21 221215" src="https://github.com/user-attachments/assets/e6e8474b-1320-491f-9c94-55aac0258739" />

<img width="1092" height="819" alt="Screenshot 2026-04-21 220407" src="https://github.com/user-attachments/assets/84579d8d-9409-4098-95a7-11785f182251" />

<img width="1090" height="557" alt="Screenshot 2026-04-21 221456" src="https://github.com/user-attachments/assets/624603e9-c28b-4134-a592-ba46d6350765" />

<img width="1096" height="1009" alt="Screenshot 2026-04-21 222607" src="https://github.com/user-attachments/assets/9f85ec4e-b970-48ef-8798-ed5ef396235f" />

<img width="1097" height="874" alt="Screenshot 2026-04-21 223555" src="https://github.com/user-attachments/assets/a60f68a8-2e15-4f6d-8cb8-97559d6d130a" />

<img width="1101" height="418" alt="Screenshot 2026-04-21 224858" src="https://github.com/user-attachments/assets/ace283a1-15ee-4a3b-b5cd-39447f9389a3" />

<img width="2547" height="1034" alt="Screenshot 2026-04-22 210938" src="https://github.com/user-attachments/assets/74219c1a-517c-4939-bc9d-2811356a29a8" />

<img width="2559" height="1113" alt="Screenshot 2026-04-22 211226" src="https://github.com/user-attachments/assets/673e9346-61ca-4625-b1a4-aeaf59272a24" />

<img width="1177" height="122" alt="Screenshot 2026-04-22 213205" src="https://github.com/user-attachments/assets/91c8e186-a930-4a97-bdc5-243e837b3df6" />

<img width="1612" height="450" alt="Screenshot 2026-06-01 205900" src="https://github.com/user-attachments/assets/38c9f9dd-6dc2-4b0a-b9de-a722a9e6cdc9" />

<img width="1973" height="1118" alt="Screenshot 2026-06-01 210843" src="https://github.com/user-attachments/assets/5665f55b-45ff-4e31-b89c-78260e346f32" />

<img width="1943" height="1087" alt="Screenshot 2026-06-01 211129" src="https://github.com/user-attachments/assets/95c77dc2-a97a-451a-9788-494322747138" />

<img width="2163" height="1060" alt="Screenshot 2026-06-01 215751" src="https://github.com/user-attachments/assets/9ffdb077-4ed1-4da2-851b-1cb33df52d61" />


## Takeaway for Security Roles
Metasploit is a powerful tool that facilitates the exploitation process. The exploitation process comprises three main steps; finding the exploit, customizing the exploit, and exploiting the vulnerable service.
