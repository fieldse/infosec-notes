tags: #forensics #reporting #legal 

- Identification
	- ensure safety, secure the scene to prevent contamination, and identify evidence to be collected 
- Collection
	- ensure authorization to collect evidence first
	- document everything collected & prove integrity
- Analysis
	- create copy of evidence for later analysis
	- uses static tools and analysis methods
	- 
- Reporting
	- after analysis, create a report of methods, tools, and findings of the investigation
	- important to document everything, so your investigation can't be discredited legally
- Legal hold
	- process where information is preserved due to expectation of potential litigation
	- servers or devices could be seized as evidence
		- Backups of data should be available, to continue operations
	- Have legal liason as central point of contact
- Timeline
	- show sequence of events on file system in graphical format

## Ethics

Analysis methods must be:
	- free of bias
	- repeatable by third parties
	- not changed or manipulated (use integrity checks, use copies of data & hard drives)

Deviation from ethical methods can result in evidence being thrown out in court

### Order of volatility
#volatility #forensics 

Evidence should be collected in order of volality, to avoid most transient evidence from becoming lost.

1. CPU & Cache:  CPU registers and cache memory
2. RAM: Contents of system memory (RAM), routing tables, ARP cache, process table, temporary swap files
3. Mass storage: Data on persistent mass storage (HDD/SDD/flash drive)
4. Log data:  Remote logging and monitoring data
5. Physical network:  Physical configuration and network topology
6. Archival media: tape backups, etc.


## Timeline reporting

tags: #timeline #reporting 

Items to include in timeline reports:

- How was access to the system obtained?
- What tools were installed?
- What file changes were made?
- What data was accessed?
- Was data exfiltrated?


## Data acquisition
tags: #data-acquisition #forensics #volatility 

Methods and tools for gathering forensic
data
- Do you have rights to search this device?
- Collect data in order of volatility

-----

## Post-incident review

## Forensic Analysis report
- final product of a forensic investigation

## Lessons learned report 
- provides details of an incident, its severity, the remediation method, and, how effective the response was

### Chain of custody report 
- the chronological documentation or paper trail recording the sequence of custody, control, transfer, analysis, and disposition of physical or electronic evidence.