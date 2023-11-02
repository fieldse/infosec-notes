
### OSI model
- Open Systems International model
- Conceptually divides computing and networks into several layers

## Data link layer
- Layer 2 of the OSI model
- Ensures data is transmitted to specific devices on a network
	- reformats data into frames
	- adds header with MAC addresses for source and destination devices

 
## Networking protocols

### TCP/IP
- Transmission Control Protocol / Internet Protocol
- Not one specific protocol, but an entire suite of protocols

### HTTP
- web traffic
- port 80

### SMTP
- Simple Mail Transfer Protocol
- Email traffic

### TCP
- Transmission Control Protocol
- connection-oriented traffic, with guaranteed delivery
- uses three-way handshake: SYN, SYN/ACK, ACK

### UDP
- User Datagram Protocol
- connectionless sessions,  does not ensure delivery

### IP 
- Internet Protocol
- Divided into [IPV4](#IPV4) and [IPV6](#IPV6)
- identifies hosts using IP addresses, in dot notation (IPV4 - ie: 192.0.0.1) or hex (IPV6)

### IPV4
- an #IP protocol
- uses 32-bit addresses with dot notation 
- Private reserved address ranges:
	- 10.x.x.x (10.0.0.0 to 10.255.255.255)
	- 172.16.x.x (172.16.0.0 to 172.31.255.255)
	- 192.168.x.x (192.168.0.0 to 192.168.255.255)
### IPV6
- an #IP protocol
- uses 128-bit addresses with hex notation
- private local network addresses:
	- prefixed with `fc00`
	- not assigned on public internet

### ICMP
 - Internet Control Message Protocol
 - Used for testing basic connectivity
 - Tools using ICMP:
	 - ping
	 - pingpath
	 - tracert
 - Often blocked, as it's used in DDOS attacks

### ARP
- Address Resolution Protocol
- part of layer 2 of the OSI model
- resolves IPV4 addresses to MAC addresses


## Media protocols

### RTP
- Real-time Transport protocol
- delivers audio and video over IP networks
- includes VOIP and streaming, push-to-talki, videoconferencing
- Not encrypted!

### SRTP
- Secure  Real-Time Transport Protocol
- encryption around RTP

### SIP
- Session Initiation Protocol (SIP)
- used to open, close, and maintain voice, video, and messaging sessions



## File transfer protocols

### FTP
- File Transfer Protocol
- transmits in cleartext
- #port 21 (control signals)
- #port 20 (data)

### SFTP
- secure version of FTP, over SSH
- uses #port 22

### TFTP
- Trivial File Transfer Protocol
- for sending small amounts of network data 
- uses UDP over #port 69


## Encryption protocols
tags: #encryption #ssl #https
### SSH
- Secure Shell
- encrypts data in transit
- uses TCP over #port 22
- used for SFTP, SCP, and other encrypted protocols


### SSL
- Secure Sockets Layer
- deprecated, older protocol for encrypting HTTP traffic or LDAP traffic
- compromised!


### TLS
- Transport Layer Security (TLS)
- replacement for SSL
- encrypts HTTP traffic to HTTPS

### IPSec
- Internet Protocol Security (IPSec)
- encrypts IP traffic: intended for IPV6, but works with IPV4
- protects #VPN traffic 


## Mail protocols
tags: #mail #email-protocol 

### SMTP
- Simple Mail Transfer Protocol
- uses #port 25 (unencrypted traffic)
- uses #port 587 (encrypted traffic)

### POP3
- Post Office Protocol v3
- transfers #email data from servers to clients


### IMAP4
- Internet Message Access Protocol v4 (IMAP4)
- Stores emails on a mail server
- allows organization and management of emails in folders
- TCP #port 143 (unencrypted connections -- Gmail)
- TCP #port 993 (encrypted connections -- Gmail)


## Directory services 

### LDAP
- Lightweight Directory Access Protocol
- specifies formats and methods to query directories
- used by Microsoft Active Directory

## Remote Access

### RDP 
- Remote Desktop Protocol (RDP)
- allows connecting to a desktop system remotely
- uses TCP  or UDP #port 3389

### OpenSSH
- suite of tools for simplifying the use of SSH to interact with remote systems
- supports SCP and SFTP

## Domain resolution
tags: #DNS

### DNS
- Domain Name System (DNS)
- resolves hostnames to IP addresses
- Types of record:
	- A record - hostname and IPV4 address
	- AAAA record - hostname an IPV6 address
	- PTR - pointer record - for reverse host lookup
	- MX - Mail exchange 
		- ordered by priority number
		- lower number is higher priority
	- CNAME - alias for a single IP address
	- SOA - start of authority
		- includes info about the DNS and its settings
		- uses TTL to determine how long clients should cache info


### DNSSEC
- DNS Security
- prevents DNS poisoning