
## Types of cryptography

-  [Symmetric](#Symmetric%20algorithms) - equal keys held by both parties, which allow both encrypting and decrypting the information
- [Asymmetric](#Asymmetric%20algorithms) - keys are split, with a public key being able to encrypt, and a private key being able to decrypt, or vice versa
- [Unbreakable](#Unbreakable%20Encryption) - truly secure encryption, the holy grail for cryptography
- [Hashing](#Hashing) - non-reversible functions for checking data integrity

## Hashing
#hashing #cryptography 
- non-reversible function
- generates a unique hash based on content of information. 
- allows verification that data is intact and hasn't been modified

### Hashing algorithms:

- SHA-1 - 160 bits, fixed output
- SHA-2 - 256 bits, fixed output
- MD5 -  128 bits, fixed output
- NTLM - 128 bits, fixed output - Microsoft's NT LAN Manager


## Symmetric algorithms
Identical keys held by both parties, which allow both encrypting and decrypting the information

- Twofish
- [AES](#AES) (Rijndael)
- [Blowfish](#Blowfish)
- [RC4](#RC4 )
- [DES](#DES)
- [3DES](#3DES)

### RC4 
- #symmetric-cryptography
-  Rivest Cipher 4
- **stream cypher**
- high speed
- considered insecure

### PGP 
- #symmetric-cryptography
- "Pretty Good Privacy"
- software suite uses primarily for encrypting email communication 
- used to sign, encrypt, and decrypt texts, emails, files, directories and disk partition
- uses  [RSA](#RSA) or [DSA](#DSA) algorithms

### AES 
- #symmetric-cryptography
- BLOCK cipher
- SYMMETRIC
-  Advanced Encryption Standard (AES), also known as Rijndael
- Developed by NIST in 2001
- block size of 128 bits, key sizes up to 256 bits
- AES-256 is considered to be [quantum resistant](#Quantum%20safety)

### Blowfish
- #symmetric-cryptography
- BLOCK cipher
- SYMMETRIC
- block size of 128 bits, key sizes up to 256 bits
- has become slower than AES

### Twofish
- todo


### DES
- #symmetric-cryptography
- Data Encryption Standard (DES)
- outdated - short key length of 56 bits
- Developed in the 1970s at IBM
  
### 3DES 
- #symmetric-cryptography
- Triple DES (3DES or TDES), officially  "Triple Data Encryption Algorithm"
- BLOCK cipher
- SYMMETRIC
- Outdated/ insecure - short key length of 56 bits

## Asymmetric algorithms
Also known as Public-key cryptography.

Keys are split into pairs, with a public key being able to encrypt, and a private key being able to decrypt, or vice versa, using one-way mathematical functions

Examples:
- [Diffie–Hellman](#Diffie–Hellman) key exchange protocol
- [DSS](#DSS) (Digital Signature Standard)
- [RSA](#RSA)
- [Elliptic-curve cryptography](#Elliptic-curve%20cryptography)
	- Elliptic Curve Digital Signature Algorithm (ECDSA)
	- Elliptic-curve Diffie–Hellman (ECDH)


### Diffie-Hellman
#asymmetric #encryption 
- mathematical method of securely exchanging cryptographic keys over a public channel
- ASYMMETRIC

### DSA
#asymmetric #encryption 
- Digital Signature Algorithm (DSA)
- a public-key cryptosystem and Federal Information Processing Standard for digital signatures
- used in SSL
- ASYMMETRIC
  
### DSS
#asymmetric #encryption 

- Digital Signature Standard (DSS)
- incorporates the Digital Signature Algorithm
- ASYMMETRIC

### Elliptic-curve cryptography
#asymmetric #encryption 

- Elliptic-curve cryptography (ECC)
- based on algebra of elliptic curves
- ASYMMETRIC
- smaller key size than other methods
- considered [quantum-vulnerable](#Quantum%20safety)
- Examples: 
	- ECDSA
	- Elliptic Curve Digital Signature Algorithm (ECDSA)
	- Elliptic-curve Diffie–Hellman (ECDH)

### RSA
#asymmetric #encryption 
- RSA (Rivest–Shamir–Adleman) 
- ASYMMETRIC
- one of the oldest public-key cryptographic systems, invented in 1977
- key length generally 1024 to 4096 bits
- used in OpenSSL
- considered [quantum-vulnerable](#Quantum%20safety)

## Unbreakable

### One-time Pad
- the only known unbreakable encryption method
- masking messages with pre-known and shared string of random characters & digits, each only used one time

## Quantum safety
- Algorithms which were originally secure prior may now be vulnerable to breaking with quantum computers
- quantum resistance - algorithms designed in a way that makes them secure against breaking with quantum computers