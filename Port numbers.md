Commonly used port numbers on the exam

Sources: 
- https://cyberkrafttraining.com/2021/08/17/the-ports-and-protocols-you-need-to-know-for-the-sy0-601-security-exam/
- https://blogs.getcertifiedgetahead.com/ports-network-security-sscp-exams/

### 21/22 - FTP
- File Transfer Protocol 
- Port: TCP 20/21
- Port 21 is the control port while port 20 is used to transfer files.

 
### 22 - SSH
- Secure Shell
- Port: TCP 22
- Designed to transmit data through a remote connection.

 
### 22 - SFTP
- Port: TCP 22
- A completely separate protocol from FTP (it is not compliant with FTP servers) that uses SSH to encrypt file transfers.

### 23 - Telnet
- insecure, deprecated
 
### 49 - TACACS+
- Port: TCP 49
- Cisco proprietary protocol used for authentication, authorization, and accounting (AAA) services

 
### 53 - Domain Name System (DNS)
 Port: UDP 53
 Used to associate IP addresses with domain names

 
### 67/68 - DHCP
- Dynamic Host Configuration Protocol (DHCP)
- Port: UDP 67/68 
- used to assign local IP addresses to devices on a network.  It is used to create multiple private IP addresses from one public IPv4 address.

### 69 - TFTP
- Trivial File Transport Protocol
- Simplified version of FPT
- Port: UDP 69

### 80 - HTTP
- Port: TCP 80 
- Protocol used for websites and most internet traffic.

### 88 - Kerberos
- Port: TCP/UDP 88 
- Network authentication protocol that allows for communication over a non-secure network.

 
### 110 - POP3
- Post Office Protocol (POP)
- Port: TCP 110 
- E-mail protocol that allows e-mail clients to communicate with e-mail servers.  POP provides only one-way communication.

### 123 - NTP
 - Network Time Protocol
 - used for synchronizing device time

### 143 / 993 - IMAP
- Internet Message Access Protocol (IMAP)
- Port: TCP 143, 993 
- E-mail protocol used by e-mail clients to communicate with e-mail servers. Provides two way communication unlike POP

 
### 161/162 - SNMP
- Simple Network Management Protocol (SNMP)
- Port: UDP 161/162
- used to monitor and manage network devices on IP networks.

 
### 389 - LDAP
- Lightweight Directory Access Protocol (LDAP)
- Port:  TCP/UDP 389
- Used to manage and communicate with directories.

### 443  - HTTPS
- Port: TCP 443 
- Secure version of HTTP that used TLS for encryption.

### 443 - SSL VPN 
- Secure Sockets Layer virtual private network
- Port: TCP 443 
 
### 445 -SMB
- Server Message Block  /  SAMBA
- Port: TCP 445
- used by Windows computers to share files, printers, serial ports, and miscellaneous communications between nodes on a network
- Uses NTLM or Kerberos for authentication

### 500 - ISAKMP
- Internet Security Association and Key Management Protocol
- VPN protocol, implements IPSEC
- Port: UDP 500
  
### 514 - Syslog
- log service utility
- Port: UDP 514

### 587 - SMTP
- SMTP (Secure Mail Transfer Protocolo) with TLS/SSL
- Port: TCP 587

### 636 - LDAPS
- Lightweight Directory Access Protocol Secure (LDAPS)
- Port: TCP 636 
- Secure version of LDAP that uses TLS for encryption

 
### 989/990 - FTPS
- File Transfer Protocol Secure (FTPS)
- Port: TCP 989/990 
- uses TLS for encryption.  It can run on ports 20/21 but is sometimes allocated to ports 989/990

 
### 993 - IMAPS
- Internet Message Access Protocol Secure 
- Port: TCP 993 
- Secure version of IMAP that uses TLS for encryption

 
### 995 - POP3S
- Post Office Protocol 3 Secure
- Port: TCP 995 
- Secure version of POP that uses TLS for encryption

### 1701 - L2TP
- Port: UDP 1701
- VPN protocol - used to create point to point connections, over UDP. 
- Needs IPSec for encryption. 
- Designed as an extension to PPTP.  

### 1723 - PPTP
 - Point-to-Point Tunneling Protocol
 - Port: TCP 1723
 - obsolete & insecure method for implementing virtual private networks

### 3868 - Diameter
- Port: 3868 
- an upgrade to RADIUS, using EAP
- Provides AAA services

### 1812 - RADIUS with EAP
- Encrypted version of RADIUS
- Port: TCP 1813 
  
### 1812/1813 - RADIUS
- Remote Authentication Dial-In User Service
- Port: UDP 1812, 1813 
- Used for authentication, authorization, and accounting (AAA) services for network services
 
### 3389 - RDP 
- Remote Desktop Protocol
- Port: TCP/UDP 3389
- Microsoft developed, provides a user with a graphical interface to connect to another computer over a network

### 5004 - SRTP
- Secure Real-time Transport Protocol
- Port: UDP 5004
- used to stream audio and video communication
- replaced RTP, adds encryption and authentication