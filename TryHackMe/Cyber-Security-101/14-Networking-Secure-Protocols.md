# TryHackMe : Networking Secure Protocols
https://tryhackme.com/room/networkingsecureprotocols

**Path:** Cyber Security 101
**Completed:** 6 April, 2026
**Difficulty:** Easy

## Overview
Learn how TLS, SSH and VPN secure your network traffic.  

## Key Skills Practised
Using Wireshark to examine unsecured and TLS secured protocols in action

## Useful Commands / Tools
- Wireshark to examine the secured traffic
- ssh username@hostname
- ssh hostname -X (for GUI support)
- sftp username@hostname
- get filename  & put filename are used once connected to the ftp site

## Screenshots


## Takeaway for Security Roles
Transport Layer Security (TLS) is added to existing protocols to protect communication confidentiality, integrity, and authenticity. Consequently, HTTP, POP3, SMTP, and IMAP become HTTPS, POP3S, SMTPS, and IMAPS, where the appended “S” stands for Secure. 
TLS offered security for HTTP without requiring any changes in the lower or higher layer protocols. In other words, TCP and IP were not modified, while HTTP was sent over TLS the way it would be sent over TCP.

Secure Shell (SSH) was created to provide a secure way to access remote systems rather than using the insecure Telnet. SSH is an extensible protocol that offers added security features for other protocols.

Protocol	Default Port Number
HTTP	80
SMTP	25
POP3	110
IMAP	143
The secure versions, i.e., over TLS, use the following TCP port numbers by default:
Protocol	Default Port Number
HTTPS	443
SMTPS	465 and 587
POP3S	995
IMAPS	993

OpenSSH offers several benefits. We will list a few key points:

Secure authentication: Besides password-based authentication, SSH supports public key and two-factor authentication.
Confidentiality: OpenSSH provides end-to-end encryption, protecting against eavesdropping. Furthermore, it notifies you of new server keys to protect against man-in-the-middle attacks.
Integrity: In addition to protecting the confidentiality of the exchanged data, cryptography also protects the integrity of the traffic.
Tunneling: SSH can create a secure “tunnel” to route other protocols through SSH. This setup leads to a VPN-like connection.
X11 Forwarding: If you connect to a Unix-like system with a graphical user interface, SSH allows you to use the graphical application over the network.

SFTP should not be confused with FTPS. FTPS is secured using TLS, just like HTTPS. While FTP uses port 21, FTPS usually uses port 990. It requires certificate setup, and it can be tricky to allow over strict firewalls as it uses separate connections for control and data transfer.
Like HTTPS, SMTPS, POP3S, IMAPS, and other protocols that rely on TLS for security, FTPS requires a proper TLS certificate to run securely.
