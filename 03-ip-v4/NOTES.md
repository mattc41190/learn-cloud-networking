# IP Address Version 4 Notes

## 4.1
- An IPv4 Address uniquely identifies a "node" / "network device" on a TCP/IP network
- An IPv4 Address is commonly represented in decimal format using a dot / "." as a delimiter
	- Ex: 81.65.200.180
- It may also be in 4 binary octets
	- Ex: 10011001 00000110 11100101 00101010

## 4.2
- We refer to IPv4 as a 32 bit number because there are 4 groups of 8 possible configurations.
	- 4 * 8 = 32
- There 2^32 possible address in IPv4
	- 4,294,967,296
- Any Octet / Decimal representation of that octet may only be up to 255
- Convert: 128.97.34.12
	- Answer: 10000000 01100001 00100010 00001100

## 4.X

- In classful IP addresses are split by octets. The latter octets provide network space, the earlier octets provide device on the network space.
	- Ex: Class A - 10.255.255.255 <-- 10 is the network space & all groups of 255 are device space on that network.
	- Ex: Class B - 10.10.255.255 <-- 10s are the network space & all groups of 255 are device space on that network. (balanced and popular)
	- Ex: Class C - 10.10.10.255 <-- 10s are the network space & the group of 255 is device space on that network.


## 4.8 

- IP addresses enable AWS resources within your VPC to communicate with one another and with external networks 