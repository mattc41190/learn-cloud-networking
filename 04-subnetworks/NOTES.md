# Subnets Notes

## 7.1

- A collision domain is a network segment where data frames may collide with one another.
- A frame (dataframe) is a digital data transmission unit in computer networking.
- A broadcast domain is a network segment where any groups of devices may reach other using broadcast traffic at Layer 2.
- Broadcast traffic, in a Layer 2 network, refers to sending traffic to all nodes on a network. 
- Layer 2 as you will recall refers to Data Link layer in OSI and is referred to as part of the Link layer by TCP model.

- A __Network Segment__ is a portion of a computer network that is separated from the rest of the network by a device such as a repeater, hub, bridge, switch or router. Each segment can contain one or multiple computers or other hosts.
- A __hub__ or repeater is a single collision and single broadcast domain
	- This means... _???_
- A __switch__ or repeater is a multi collision (one per port) and single broadcast domain (one per switch)
	- This means... _???_
- A __router__ is a multi collision (one per port) and multi broadcast domain (one per port)
	- This means... _???_

- Resources:
	- https://en.wikipedia.org/wiki/Frame_(networking)
	- https://www.juniper.net/documentation/en_US/junos/topics/concept/broadcast-qfx-series-understanding.html
	- https://www.inetdaemon.com/tutorials/basic_concepts/network_models/TCP-IP_model/
	- http://www.linfo.org/network_segment.html

## 7.2

- A __Subnet__ is an identifiably separate part of a network (network segment?)
- Network engineers employ subnetworks (subnets) to partition (separate) networks into logical subnets.
- Benefits of Subnetting: Security, Efficiency, and Address Space Management Simplicity. 
- Subnetting occurs at layer 3 of the OSI model (The Network Layer) with Routers.

## 7.3

- In IPv4 the most common reason for subnetting is to overcome the very limited address provsioned by IPv4.
- With subnetting several custom made networks maybe created from a larger more generic network block.
- A subnet forms a broadcast domain as each network device has the same network ID.
- Subnets with routers are more secure as traffic may be inspected in the router.

## 7.6

- An IP Address is composed of two parts, a network ID and a device addresses section.
- A Class A address has 16 million unique device ID possibilities 
- A Class A address with a network ID of 10 may house the possible sets.
	- 10.0.0.0 to 10.255.255.255 or 00001010.00000000.00000000.00000000 to 00001010.11111111.1111111.11111111
- 16 million unique device ID talking on the same broadcast domain leaves the likelihood for collisions too high
	- The solution is to partition a network into subnets
- Subnets take device address and reserves them.
	- In the Class Network ID 10 example above the network maybe subnetted into 8 networks by making the following reservation:
		- Subnet A
		- 00001010.11100000.00000000.00000000 to 00001010.11111111.1111111.11111111
		- Subnet B
		- 00001010.01100000.00000000.00000000 to 00001010.01111111.1111111.11111111
		- Subnet C
		- 00001010.00100000.00000000.00000000 to 00001010.00111111.1111111.11111111
		- Subnet D
		- 00001010.10000000.00000000.00000000 to 00001010.10011111.1111111.11111111
		- Subnet E
		- 00001010.11000000.00000000.00000000 to 00001010.11011111.1111111.11111111
		- Subnet F
		- 00001010.10100000.00000000.00000000 to 00001010.10111111.1111111.11111111
		- Subnet G
		- 00001010.00000000.00000000.00000000 to 00001010.00011111.1111111.11111111
		- Subnet H
		- 00001010.01000000.00000000.00000000 to 00001010.01011111.1111111.11111111


