
## Types of cryptography

-  [Symmetric](#Symmetric%20algorithms) - equal keys held by both parties, which allow both encrypting and decrypting the information
- [Asymmetric](#Asymmetric%20algorithms) - keys are split, with a public key being able to encrypt, and a private key being able to decrypt, or vice versa
- [Unbreakable](#Unbreakable%20Encryption) - truly secure encryption, the holy grail for cryptography


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
-  Advanced Encryption Standard (AES), also known as Rijndael
- Developed by NIST in 2001
- block size of 128 bits, key sizes up to 256 bits
- AES-256 is considered to be [quantum resistant](#Quantum%20safety)

### Blowfish
- #symmetric-cryptography
-  symmetric block cipher  
- block size of 128 bits, key sizes up to 256 bits
- has become slower than AES

### DES
- #symmetric-cryptography
- Data Encryption Standard (DES)
- outdated - short key length of 56 bits
- Developed in the 1970s at IBM
  
### 3DES 
- #symmetric-cryptography
-  Triple DES (3DES or TDES)
- officially  "Triple Data Encryption Algorithm"
- symmetric block cipher
- outdated - short key length of 56 bits

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
- mathematical method of securely exchanging cryptographic keys over a public channel

### DSA
- Digital Signature Algorithm (DSA)
- a public-key cryptosystem and Federal Information Processing Standard for digital signatures
- used in SSL
  
### DSS
- Digital Signature Standard (DSS)
- incorporates the Digital Signature Algorithm

### Elliptic-curve cryptography
- Elliptic-curve cryptography (ECC)
- public-key cryptography based on the algebraic structure of elliptic curves
- smaller key size than other methods
- considered [quantum-vulnerable](#Quantum%20safety)
- Examples: 
	- ECDSA
	- Elliptic Curve Digital Signature Algorithm (ECDSA)
	- Elliptic-curve Diffie–Hellman (ECDH)

### RSA
- RSA (Rivest–Shamir–Adleman) 
- one of the oldest public-key cryptographic systems, invented in 1977
- key length generally 1024 to 4096 bits
- used in OpenSSL
- considered [quantum-vulnerable](#Quantum%20safety)

## Unbreakable

### One-time Pad
- the only known unbreakable encryption method
- masking messages with pre-known and shared string of random characters & digits, each only used one time
## Hashing
#hashing #cryptography 
- non-reversible function
- generates a unique hash based on content of information. 
- allows verification that data is intact and hasn't been modified
### Hashing algorithms:

- SHA-1
- SHA-2
- MD5

## Quantum safety
- Algorithms which were originally secure prior may now be vulnerable to breaking with quantum computers
- quantum resistance - algorithms designed in a way that makes them secure against breaking with quantum computers