
## Network types

### Intranet vs Extranet
- Intranet - internal network
- Extranet - segment of network that can be accessed from outside

### Screened Subnet
- DMZ (Demilitarized Zone)
- intermediary network segment between untrusted outside traffic and trusted internal traffic

### VLANs
- Virtual Local Area Network (VLAN)
- groups several networks into a single virtual network
- can be inside or outside the physical network

## Domain resolution
tags: #DNS

### DNS servers
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
- DNSSEC (DNS Security) - enhanced security methods for DNS records, prevents DNS poisoning
- adds cryptographic signatures to existing DNS records
- digital signatures are stored in DNS name servers alongside common record types
- Example fields:
	- **RRSIG** - Contains a cryptographic signature
	- **DNSKEY** - Contains a public signing key
	- **DS** - Contains the hash of a DNSKEY record

## Gateways

### Network Address Translation Gateway (NAT)
- NAT - protocol for translating public IPs to internal private IPs and vice-versa
- NAT gateway hosts NAT service
	- Hides internal IPs from public internet
- Static vs Dynamic
	- Static: single public IP for 1-1 mapping
	- Dynamic: multiple public IPs, one-to-many mapping

## Routers and Proxies
tags: #proxy #router #load-balancing

### Router
- connects multiple network segments into a single network, and routes traffic between segments
### Access Control Lists (ACL)
- rules on router or firewall determining which traffic should be passed or denied
- packet-level filtering, based on:
	- IP address
	- ports
	- porotocol numbers

### Proxy servers
- Intermediary host, performs redirection of traffic
-  can perform caching
- transparent vs non-transparent:
	- transparent - passes traffic without modification
	- non-transparent - can filter or modify requests
### Reverse proxy
- Also know as load balancer
- lives in screened subnet
- can perform load-balancing 

- DNSSEC (DNS Security)
## Network security
- digital signatures are stored in DNS name servers alongside common record types
tags: #security #firewall

### Physical Isolation
- Air-gapping

### Logical Separation
- non-physical (ie: programmatic) separation and segmentation of networks

### Firewalls
- Filters incoming & outgoing traffic for a network or single host

Firewall types:
- Host-based - monitors traffic for a single host
- Software based vs Hardware based
- Stateless or Stateful
	- Stateless: uses ACL rules to identify traffic
	- Stateful:  
		- tracks ongoing sessions
		- makes decisions based on traffic context or state
- Web application firewall (WAF)
	- filters for a single web application
- Next-Gen Firewall (NGF)
	- advanced firewall
	- peforms deep-packet inspection

### Unified Threat Management
- UTM
- combines multiple security functions in one:
	- URL filtering
	- malware inspection
	- content inspection
	- DDOS mitigation

### Jump Server
- AKA "jump box"
- hardened server within another network segment
- provides secure launching point within a different security zone