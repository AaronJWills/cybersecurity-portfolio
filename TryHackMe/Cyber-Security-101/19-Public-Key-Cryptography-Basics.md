# TryHackMe : Public Key Cryptography Basics
https://tryhackme.com/room/publickeycrypto

**Path:** Cyber Security 101
**Completed:** 12 April, 2026
**Difficulty:** Easy

## Overview
How public key ciphers such as RSA work and their role in applications such as SSH.

## Key Skills Practised
- RSA CTF's
- Key exchange algorithm maths (inc Diffie-Hellman Key Exchange)
- Checking SSH keys
- Decrypting messages using GPG

## Useful Commands / Tools
- gpg --full-gen-key
- gpg --import backup.key to import your key from backup.key
- gpg --decrypt confidential_message.gpg to decrypt your messages
- ssh ipaddress
- ssh-keygen
- ssh-keygen -t ed25519
- ssh -i privateKeyFileName user@host
- https://github.com/Ganapati/RsaCtfTool
- https://github.com/ius/rsatool
  

## Screenshots


## Takeaway for Security Roles
Core Security Principles:

Authentication: Confirming the identity of the communicating party.
Authenticity: Verifying that the message genuinely comes from the claimed sender.
Integrity: Ensuring data is not altered during transmission.
Confidentiality: Preventing unauthorized access to sensitive information.
Cryptography Applications:

Symmetric Encryption: Fast and efficient for confidentiality but requires secure key sharing (e.g., AES).
Asymmetric Encryption: Slower but essential for authentication, integrity, and secure key exchange (e.g., RSA, Diffie-Hellman).
Key Exchange:

Diffie-Hellman: Establishes a shared secret over insecure channels for symmetric encryption without pre-existing shared secrets.
RSA:

Relies on the difficulty of factoring large numbers for secure communication.
Used for encryption, digital signatures, and secure key exchange.
Real-World Use:

Digital signatures and certificates verify identities and ensure secure communication.
Asymmetric cryptography is often used to negotiate symmetric encryption keys for faster communication.
CTF Relevance:

Cryptography challenges often involve breaking RSA or Diffie-Hellman implementations using known variables like p, q, n, e, and d.

Server Authentication:

SSH clients verify server identity using public key fingerprints to prevent man-in-the-middle attacks.
Once confirmed, the server’s public key is stored for future silent authentication.
Client Authentication:

SSH key-based authentication is more secure than passwords, using public/private key pairs.
Private keys must remain confidential and can be encrypted with a passphrase for added security.
Digital Signatures:

Ensure authenticity and integrity of digital messages or documents using asymmetric cryptography.
Private keys are used to sign, and public keys verify the signature.
Certificates:

TLS certificates authenticate websites and enable HTTPS.
Certificates rely on a chain of trust established by Certificate Authorities (CAs).
PGP/GPG:

Used for encrypting files and emails, and for digital signing to ensure confidentiality and integrity.
Public keys are shared for encryption, while private keys are used for decryption.
Key Management:

Always back up private keys securely and use strong passphrases to protect them.
Tools like ssh-keygen and gpg facilitate key generation and management.

