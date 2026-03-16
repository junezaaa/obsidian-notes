#pgtablestruct 

	Track all physical pages instead of logical pages

- One entry for each real page of memory.
- Decreases memory needed to store each pg table, but increase search time needed when a page reference occurs.
- Use hash table to limit the search to one, or at most a few.
	- TLB can accelerate access
![[Pasted image 20260314015232.png|489]]