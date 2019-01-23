# Subnets Notes

## 7.1

- A collision domain is a network segment where data frames may collide with one another.
- A frame (dataframe) is a digital data transmission unit in computer networking.
- A broadcast domain is a network segment where any groups of devices may reach other using broadcast traffic at layer 2.
- Broadcast traffic, in a Layer 2 network, broadcasting or broadcast traffic refers to sending traffic to all nodes on a network. 
- Layer 2 as you will recall refers to Data Link layer in OSI and is referred to as part of the Link layer by TCP model.


- A __hub__ or repeater is a single collision and single broadcast domain
	- This means...
- A __switch__ or repeater is a multi collision (one per port) and single broadcast domain (one per switch)
	- This means...
- A __router__ is a multi collision (one per port) and multi broadcast domain (one per port)
	- This means...

- Resources:
	- https://en.wikipedia.org/wiki/Frame_(networking)
	- https://www.juniper.net/documentation/en_US/junos/topics/concept/broadcast-qfx-series-understanding.html
	- https://www.inetdaemon.com/tutorials/basic_concepts/network_models/TCP-IP_model/