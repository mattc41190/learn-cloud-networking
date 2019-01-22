# Network Communication Systems Notes

## Course Section 2.1
- Signal transmission has three essential components.
	- Transmitter
	- Relay(s)
	- Receiver
- To ensure compatibility and fault tolerance/recovery network communication models were created
- Popular defunct models include IBM's SNA protocol and DECNET.
- Today we use the OSI and TCP/IP models.

## Course Section 2.2
- Open Systems Interconnection -- OSI
- The purpose of a network communication model (*protocol*) is to:
	- Characterize - Clearly describe what is being communicated.
	- Standardize - Ensure all parties share a common definition of terms.
	- Abstract - Reduce mental overheard.
- The ISO-OSI network communications model is visualized as unique 7 layers and its goal is the interoperability of diverse systems via a standard protocol.
- The seven layers of the OSI model are:

| Layer | Name | Format | Function | Example Protocol | Address Type |
|-------|--------------|--------------------------------------|-----------------------------|-------------------|--------------|
| 1 | Physical | Bit | Raw bits on physical medium | TIA-323-F, DOCSIS | N/A |
| 2 | Data Link | Frame | Node-To-Node Communication | MPLS | MAC Address |
| 3 | Network | Packet | Routing and addressing | IP, IGMP | IP Address |
| 4 | Transport | Protocol Data Unit  (PDU) -- Segment | End-To-End Integrity | TCP, UDP | Port |
| 5 | Session | Data | Connection Dialog | SOCKS, RPC | Socket |
| 6 | Presentation | Data | Data Representation | XDR, SMB | Hostname |
| 7 | Application | Data | Interactions with user | FTP | Hostname |

- The TCP/IP model roughly maps the OSI model in broader terms.
	- Layers 1 and 2 are called the `Link` layer
	- Layer 3 is the `Internet` layer
	- Layer 4 is the `Transport` layer 
	- Layers 5 through 7 are called the `Application` layer

- Resources:
	- https://www.versatek.com/blog/you-wont-believe-what-the-osi-model-and-pizza-have-in-common/
	- https://en.wikipedia.org/wiki/OSI_model

## Course Section 2.4

- Popular Port Numbers:
	- 21 - FTP
	- 22 - SSH
	- 53 - DNS
	- 80 - HTTP
	- 443 - HTTPS
	- 2049 - NFS
	- 3306 - Aurora

- Port Number Ranges:
	- 0 to 1023: Well-known / system ports (privileged access only)
	- 1024 to 49,151: User registered ports (user determined access)
	- 49,152 to 65,535: Dynamic ports (used dynamically by application / nondeterministic)

## Course Section 2.6 

- A TCP/IP connections consists of 2 endpoints. 
- Each endpoint is a collection of an IP Address and a Port number
- The `source` IP will be your computer's IP and the `source` port will usually be a dynamic or ephemeral port (see port ranges).
- The `destination` will be unknown until DNS does a lookup, but the `destination` port will be a well known system port (see port ranges). 

## Tasks

- Write Terraform configurations that:
	- Create Network ACLs
	- Create Security Groups
	- Associate the Network ACL you created to a Subnet
	- Associate the security group you created to an instance running in the subnet to which the NACL is associated
	- Run your configuration by a network expert
