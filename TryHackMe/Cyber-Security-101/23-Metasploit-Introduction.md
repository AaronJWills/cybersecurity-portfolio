# TryHackMe : Metasploit Introduction
https://tryhackme.com/room/metasploitintro

**Path:** Cyber Security 101
**Completed:** 21 March, 2026
**Difficulty:** Easy

## Overview
The Metasploit Framework is a set of tools that allow information gathering, scanning, exploitation, exploit development, post-exploitation, and more. While the primary usage of the Metasploit Framework focuses on the penetration testing domain, it is also useful for vulnerability research and exploit development.

Modules are small components within the Metasploit framework that are built to perform a specific task, such as exploiting a vulnerability, scanning a target, or performing a brute-force attack.
Auxiliary-supporting modules such as scanners, crawlers & fuzzers
Encoders-encode the exploit and payload to help signature based AV miss them
Evasion-these modules will try to directly attempt to evade AV
Exploits-code that uses a vulnerability
NOPs-used as a buffer to get a consistent size payload
Payloads-code that runs on the target system.  Types of payloads are Adapters (wraps a payload to convert it into a different format), Singles (self contained payloads), Stagers (set up connections to targets to then download the rest later), Stages (downloaded by the stager).
Post-post-exploitation modules


## Key Skills Practised
Learning Metasploit commands and help systems
Launching Metasploit
Setting options
Running exploits
Switching sessions

## Useful Commands / Tools
msfconsole - launches the Metasploit console
help
history
search
use
show options
set
exploit / run
background / CTRL+Z
sessions



## Screenshots


## Takeaway for Security Roles
Metasploit is a powerful tool that facilitates the exploitation process. The exploitation process comprises three main steps; finding the exploit, customizing the exploit, and exploiting the vulnerable service.
