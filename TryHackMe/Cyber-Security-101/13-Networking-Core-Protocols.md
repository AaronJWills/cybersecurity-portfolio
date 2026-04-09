# TryHackMe : Networking Core Protocols
https://tryhackme.com/room/networkingcoreprotocols

**Path:** Cyber Security 101
**Completed:** 4 April, 2026
**Difficulty:** Easy

## Overview
Learn about the core TCP/IP protocols

## Key Skills Practised
- WHOIS, DNS, HTTP, FTP, SMTP, POP3 and IMAP

## Useful Commands / Tools
- nslookup 
- whois
- GET / HTTP/1.1  &  Host:anything    GET /file.html HTTP/1.1
- ftp *machinename*

## Screenshots


## Takeaway for Security Roles
Examined common networking protocols and how they work behind the scenes, showing the magic that applications usually hide

DNS - 
A record: The A (Address) record maps a hostname to one or more IPv4 addresses. 
AAAA Record: The AAAA record is similar to the A Record, but it is for IPv6.
CNAME Record: The CNAME (Canonical Name) record maps a domain name to another domain name. 
MX Record: The MX (Mail Exchange) record specifies the mail server responsible for handling emails for a domain.

HTTP -
GET retrieves data from a server, such as an HTML file or an image.
POST allows us to submit new data to the server, such as submitting a form or uploading a file.
PUT is used to create a new resource on the server and to update and overwrite existing information.
DELETE, as the name suggests, is used to delete a specified file or resource on the server.
Once connected to a web server via telnet you can display the page with the GET command

FTP - 
USER is used to input the username
PASS is used to enter the password
RETR (retrieve) is used to download a file from the FTP server to the client.
STOR (store) is used to upload a file from the client to the FTP server.

SMTP -
HELO or EHLO initiates an SMTP session
MAIL FROM specifies the sender’s email address
RCPT TO specifies the recipient’s email address
DATA indicates that the client will begin sending the content of the email message
. is sent on a line by itself to indicate the end of the email message
You could use telnet on port 25 to connect to a mail server to send an email

POP3 -
USER <username> identifies the user
PASS <password> provides the user’s password
STAT requests the number of messages and total size
LIST lists all messages and their sizes
RETR <message_number> retrieves the specified message
DELE <message_number> marks a message for deletion
QUIT ends the POP3 session applying changes, such as deletions
You could if you wanted to connect to a mail server on port 110 and retrieve your POP email

IMAP - 
LOGIN <username> <password> authenticates the user
SELECT <mailbox> selects the mailbox folder to work with
FETCH <mail_number> <data_item_name> Example fetch 3 body[] to fetch message number 3, header and body.
MOVE <sequence_set> <mailbox> moves the specified messages to another mailbox
COPY <sequence_set> <data_item_name> copies the specified messages to another mailbox
LOGOUT logs out
