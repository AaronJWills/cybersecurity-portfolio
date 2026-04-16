# TryHackMe : Hashing Basics
https://tryhackme.com/room/hashingbasics

**Path:** Cyber Security 101
**Completed:** 14 April, 2026
**Difficulty:** Easy

## Overview
Hashing functions and their uses in password verification and file integrity checking

## Key Skills Practised
- Calculating hashes
- Identifying hash types
- Cracking hashes / passwords

## Useful Commands / Tools
- md5sum, sha1sum, sha256sum, and sha512sum
- https://crackstation.net/
- https://hashes.com/en/decrypt/hash
- https://hashcat.net/hashcat/
- https://www.openwall.com/john/
- hashcat -m <hash_type> -a <attack_mode> hashfile wordlist
- For example, hashcat -m 3200 -a 0 hash.txt /usr/share/wordlists/rockyou.txt will treat the hash as Bcrypt and try the passwords in the rockyou.txt file.
- https://hashcat.net/wiki/doku.php?id=example_hashes
- 

## Screenshots


## Takeaway for Security Roles

- $y$	yescrypt is a scalable hashing scheme and is the default and recommended choice in new systems
- $gy$	gost-yescrypt uses the GOST R 34.11-2012 hash function and the yescrypt hashing method
- $7$	scrypt is a password-based key derivation function
- $2b$, $2y$, $2a$, $2x$	bcrypt is a hash based on the Blowfish block cipher originally developed for OpenBSD but supported on a recent version of FreeBSD, NetBSD, Solaris 10 and newer, and several Linux distributions
- $6$	sha512crypt is a hash based on SHA-2 with 512-bit output originally developed for GNU libc and commonly used on (older) Linux systems
- $md5	SunMD5 is a hash based on the MD5 algorithm originally developed for Solaris
- $1$	md5crypt is a hash based on the MD5 algorithm originally developed for FreeBSD
- Hashing Basics:

A hash function generates a fixed-size output (hash value) from input data of any size.
Hashing ensures data integrity by detecting even the smallest changes in input data.
Hash functions are one-way operations, making it computationally impractical to reverse the process.
Importance of Hashing:

Used to verify file integrity (e.g., comparing downloaded files to originals).
Protects passwords by storing their hash values instead of plaintext.
Hash Collisions:

Occur when two different inputs produce the same hash value.
Modern algorithms like SHA-256 minimize collision risks, while older ones like MD5 and SHA-1 are insecure due to known vulnerabilities.
Password Storage Best Practices:

Use secure hashing algorithms (e.g., Argon2, Bcrypt, Scrypt) with unique salts to protect against rainbow table attacks.
Avoid storing passwords in plaintext or using deprecated algorithms like SHA-1.
Salting:

Adding a unique, random value (salt) to passwords before hashing ensures that identical passwords produce different hash values.
Salts do not need to be kept private and are stored alongside the hash.
Encryption vs. Hashing for Passwords:

Hashing is preferred for password storage because it avoids the need to store decryption keys, which could compromise all passwords if leaked.
Real-World Applications:

Hashing is used in authentication systems, file integrity checks, and protecting against data tampering.

Hashing for Passwords:

Hashing secures passwords by storing their hash values instead of plaintext.
Use secure algorithms like Argon2, Bcrypt, or Scrypt with unique salts to protect against rainbow table attacks.
Avoid insecure practices like storing passwords in plaintext, using deprecated encryption, or insecure hash functions like MD5 or SHA-1.
Hash Cracking:

Tools like Hashcat and John the Ripper are used to crack hashes by comparing hashed inputs to target hashes.
GPUs accelerate hash cracking, but algorithms like Bcrypt resist GPU-based attacks.
Context and research are essential for identifying hash types, especially when automated tools are unreliable.
File Integrity Checking:

Hashing ensures files haven’t been modified by comparing their hash values to the original.
Useful for verifying downloaded files and detecting duplicate files.
HMAC (Keyed-Hash Message Authentication Code):

Combines hashing with a secret key to ensure authenticity and integrity of data.
Used in secure communication to verify the sender and prevent tampering.
Linux and Windows Password Hashes:

Linux stores password hashes in /etc/shadow with prefixes indicating the hashing algorithm (e.g., yescrypt, bcrypt, SHA-512).
Windows uses NTLM hashes stored in the SAM file, which can be extracted using tools like mimikatz.
Best Practices:

Always use modern hashing algorithms and unique salts for password storage.
Regularly verify file integrity using hashing to prevent tampering or corruption.
