How to allocate a **n size part** from a list of free holes?
- **First-fit**: first-hole that is big enough.
	- If given that n blocks are allocated, then n/2 blocks are lost to fragmentation. 50% rule.
- **Best-fit:** Smallest-hole that is big enough; must search the entire list if unordered.
- **Worst-fit:** Biggest-hole; must also search the entire list if unordered.