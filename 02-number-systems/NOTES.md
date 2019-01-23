# Number Systems Notes

## 3.1

- Numeral system are useful for IP addresses
- Being able to convert binary, hexadecimal, and decimal is useful when partitioning networks into sub-networks (subnets).
- Positional number systems use a symbol and a placement to denote value. 
	- Example in Decimal: 159
	- 9 is in the one spot 
	- 5 is in the ten spot
	- 1 is in the hundred spot

## 3.2
- Common Uses For Different Bases:
	- Sexagesimal (Base 60): Time Series & Trigonometry (0-59)
	- Hexadecial (Base 16): IPv6 (0-16)
	- Decimal (Base 10): IPv4 (0-10)
	- Binary (Base 2): Computing (0-1)

## 3.3 
- Base 10 has 10 unique symbols:
	- (0,1,2,3,4,5,6,7,8,9)
	- 0-9 <- first position notation
	- 10-99 <- second position notation
	- 100-999 <- third position notation
	- So on...

- Using positional exponents we can determine the value of any number.
- Rules: Base 10 exponent to the positional power * the number in that spot
	- 2345
	- 5 == 5 * 10 ^ 0 == 5 +
	- 4 == 4 * 10 ^ 1 == 40 +
	- 3 == 3 * 10 ^ 2 == 300 +
	- 2 == 2 * 10 ^ 3 == 2000 = 2345

## 3.5
- Base 16 has 16 unique symbols
	- (0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F) 
- Hex /  Base 16 is often prefixed with `ox`
- Rules: Base 16 has each value multiplied by 16 to the positional power
	- oxEF
	- F == 15 * 16 ^ 0 == 15 +
	- E == 14 * 16 ^ 1 == 224 = 239

### Missing Several Conversion Sections That I Was too Embarrassed To Do At Work

## 3.10

- IPv4 is commonly represented in decimal format
	- Ex: 80.232.24.57
- In theory each value delimited by a dot could be a decimal number between 0 and 255
- IPv6 is commonly represented in hexadecimal format
- In theory each value delimited by a colon could be any decimal number between 0 and 65535 

