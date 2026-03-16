#pgtablestruct 
- Common in addr > 32 bits
- The virtual pg number is hashed into a pg table.
	- Contains a chain of elements hashing to the same location
	- Each element contains
		1. The virtual pg no.
		2. the value of the mapped page frame
		3. a pointer to the next element
- *Virtual pg no. are compared in this chain searching for a matching corresponding physical frame to be extracted.*
![[Pasted image 20260314014229.png|527]]