# OSI Model

The OSI  (Open Systems International) model is a conceptual framework for separating levels of computing and networks into abstract categories.

Developed by International Organization for Standardization (ISO)

Conceptually divides computing and networks into the following seven layers:
	1. Physical Layer
	2. Data Link layer
	3. Network layer
	4. Transport layer
	5. Session layer
	6. Presentation layer
	7. Application layer

### Layer 1: Physical Layer
- Data Unit: Bit, Symbol
- Transmission and reception of raw bit streams over a physical medium

### Layer 2: Data Link layer
- Data Unit: Packet
- Ensures data is transmitted to specific devices on a network
	- reformats data into frames
	- adds header with MAC addresses for source and destination devices

### Layer 3: Network layer
- Data Unit: Frame
- Structuring and managing a multi-node network, including addressing, routing and traffic control

### Layer 4: Transport layer
- Data Unit: Segment, Datagram
- Reliable transmission of data segments between points on a network, including segmentation, acknowledgement and multiplexing

### Layer 5: Session layer
- Data Unit: Data
- Managing communication sessions, i.e., continuous exchange of information in the form of multiple back-and-forth transmissions between two nodes

### Layer 6: Presentation layer
- Data Unit: Data
- Translation of data between a networking service and an application; including character encoding, data compression and encryption/decryption

### Layer 7: Application layer
- Data Unit: Data
- High-level protocols such as for resource sharing or remote file access, e.g. HTTP
