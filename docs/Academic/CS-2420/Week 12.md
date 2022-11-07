## Hash Stuff

### Keywords:
#### Hash Table
	- DS that stores unordered items into a location in an array
#### Key
	- First item in key pair value, used to map to an index
#### Bucket
	- Each element in the array is a bucket
#### Collision
	- Numbers can have same hash values, and end up being mapped to the same location. Can be resolved with chaining or open addressing
#### Chaining
	- Items that map to the same bucket can be stored by using a structure in that bucket
#### Open Addressing
	- Linear Probe 
	- Quadratic Probe
	- Double Hash
#### Resizing
	- Load Factor = items / buckets
#### Clustering
#### Hash Functions (computes the correct location)
	- Modulo Hash
		- key % size_of_array
	- Mid-square hash
	- Mid-square with binary
	- Multiplicative string hash function
#### Direct Hashing
	- Always provides O(1) time complexity, but creates O(n+1) or O(n) space complexity because each key gets mapped to its direct index value. No collisions, but takes a TON of space

### Applications
Cryptography
Data integrity (integrity can't be garanteed, but but corruption can be garanteed)