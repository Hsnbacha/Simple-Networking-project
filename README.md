Given Network addresses 192.168.40.0 

No. of subnets = 2

2'N= no. of subnets ===== 2'N=2   (' is to the power)

N=1

255.255.255.255 4 octets / 8 bits

And here we should borrow 1 bit for the network part

So the first octet will contain 8 bits

11111111.11111111.11111111.10000000
Here we should use the number of borrowed bits to calculate the subnet mask so according to that we borrowed 1 bit. The meaning of that , the first  3 octet will have completely 1 and the last fourth octet we have the first one only and the others are 0 according to 1 2 4 8 16 32 64 128

Then we need to convert this binary (11111111.11111111.11111111.10000000) into decimals :

11111111.11111111.11111111.10000000

255.255.255. 128 => subnet mask	

Based on block size subnet mask 2 raised to power 0 and we start counting zero from right to left until we end up in the last zero which will be 2 to the power 7 = 128 

And here we will have the subnet mask

The block size is 128. So the blockers basically will tell us how to move from one subject to another. The block size will act as a step from this subnet to another subject.
Starting from the first Segment:

1st Subnet :

Subnet mask= 255.255.255. 128	

Network ID= 192.168.40.0  First Subnet starts from zero

Range of valid hosts = 192.168.40.1 --- 192.168.40.126

Broadcast ID= 192.168.40.127 Broadcast ID will be the last IP address. And It will be 127 because from 0 to 127 there will be 128.

‘’’’’’ (How to calculate a slash notation from a decimal subnet mask 4 octet first 3 octet are 24 and the borrowed 1 is the 25) then the slash notation is 25 if we have 255.255.255.128





2nd Subnet :

Subnet mask= 255.255.255.128 The subnet mask will remain the same

Network ID= 192.168.40.128

Range of valid hosts = 192.168.40.129 --- 192.168.40.254

Broadcast ID= 192.168.40.255   after adding 128 to the network ID the Broadcast will be 255 . 

128+128 and subtract 1 because we have used 128 so starting from 129

And here we start configuration according to what topology we have created 



Subnet mask     block size

128	------------------		128

192	------------------		64

224	------------------		32

240	------------------		16

248	------------------		8

252	------------------		4

254	------------------		2

255	------------------		1



