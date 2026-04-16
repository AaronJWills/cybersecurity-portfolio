# TryHackMe : John the Ripper The Basics
https://tryhackme.com/room/johntheripperbasics

**Path:** Cyber Security 101
**Completed:** 15 April, 2026
**Difficulty:** Easy

## Overview
How to use John the Ripper, a powerful and adaptable hash-cracking tool.

## Key Skills Practised
- Cracking Windows authentication hashes
- Crack /etc/shadow hashes
- Cracking password-protected Zip files
- Cracking password-protected RAR files
- Cracking SSH keys

## Useful Commands / Tools
- john [options] [file path]
- john --wordlist=[path to wordlist] [path to file] (Automatic cracking)
- https://hashes.com/en/tools/hash_identifier
- https://gitlab.com/kalilinux/packages/hash-identifier/-/tree/kali/master
- john --format=[format] --wordlist=[path to wordlist] [path to file] eg. john --format=raw-md5 --wordlist=/usr/share/wordlists/rockyou.txt hash_to_crack.txt  (format specific cracking)
- john --list=formats
- unshadow [path to passwd] [path to shadow]  eg. unshadow local_passwd local_shadow > unshadowed.txt
- john --single --format=[format] [path to file]
- john --wordlist=[path to wordlist] --rule=PoloPassword [path to file]  (using custom password rules)
- zip2john [options] [zip file] > [output file]  (convert the Zip file into a hash format that John can understand)
- rar2john [rar file] > [output file]  (convert the RAR file into a hash format that John can understand)
- ssh2john [id_rsa private key file] > [output file]   or  /opt/john/ssh2john.py id_rsa > id_rsa_hash.txt
- 

## Screenshots


## Takeaway for Security Roles

