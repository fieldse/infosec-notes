### IPSec
- a  TCP/IP #encryption protocol 
- used by [l2tp](#l2tp)
- uses [IKE](#ike) for key exchange

### IKE
- Internet Key Exchange
- method for secure key exchange when setting up a secure tunnel


### PPP
- Point to point protocol
- #vpn protocol
- #port: 


### PPTP
- Point to point tunneling protocol
- #vpn protocol
- #port: 1723
- Encapsulates & encrypts [PPP](#ppp) packets 
- uses CHAP authentication, vulnerable to attack. 

### L2TP
- Layer 2 tunneling protocol
- #vpn protocol
- #port: 1701
- connection between two devices not on same network
- stronger than [pptp](#pptp)
- not encrypted by default: paired with [IPSEC](#ipsec)
	

### Secure Association (SA)
- establishing secure connections by keys or certificates

###  Authentication Header (AH)
- Header information of the packets used in [IPSec](#ipsec)
- provides authenticity & integrity

### ESP 
- Encapsulating Security Payload
- more secure than just [AH](#Authentication-Header)
- encapsulates, encrypts, & authenticates content of the IPSec packets
- Tunnel mode & transport mode
	- tunnel - for outside connections, totally encrypted
	- transport - for internal networks, leaves headers visible