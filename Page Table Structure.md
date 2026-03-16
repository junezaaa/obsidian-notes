#pgtablestruct
Memory structure for paging can get huge using straight-forward methods
	- Consider a 32-bit logical addr
		- [[Logical vs Physical Address Space#^690536|Logical addr space]] is of 2^32 = 2^2 x 2^30 in bytes (4GB, *1 GB = 2^30 bytes*)
	- Page size of 4KB(2^10 bytes) = 2^12 in bytes.
	- Number of entries in the [[Address Translation Scheme|pg table]] is 2^32 div by 2^12 = 2^20 bytes
	- If each page table entry is 4 bytes
		- Pg table size is 2^22 bytes

There are 3 types of structure:
	1. [[Hierarchical Paging]]
	2. [[Hashed Page Table]]
	3. [[Inverted Page Table]]