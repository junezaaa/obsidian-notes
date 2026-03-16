- Small page size:
	- less [[Internal vs External Fragmentation|internal frag]]
	- more pg required per proc
	- larger pg table (no in RAM always)
- Large size:
	- Large num of pg in main mem; the mem will contain portions of the proc near recent ref as time goes on ;Low [[page fault]]
	- Increase size cause pages to contain location further from the recent ref. high pg fault
	- Page size approaching the size of the program: pg fault low again
![[Pasted image 20260315151338.png|651]]
- Disk designed to efficiently transfer large blocks
	- Favors large page size.

#EAT 
- Overhead due to pg table and internal fragment
	Overhead = ![[Pasted image 20260315151558.png|57]] (s/p = amount of virtual pg)
		- s = average proc size in bytes
		- p = page size in bytes
		- e = page entry length in bytes
- Optimized when p = sqrt(2se)
- Multiple page sizes provide the flexibility needed (to use [[Translation Lookaside Buffer]] efficiently)  
	- Large pages can be used for program instructions
	- Small pages can be used for threads