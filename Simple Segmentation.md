#mmtech 
- Each proc is divided into no. of segments.
- A process is loaded by loading all of its segments into [[Dynamic Partitioning|dynamic partition]] that need not be contiguous.

Strength:
	- No internal frag
	- Improve mem util and reduce overhead compared to [[Fixed Partitioning|fixed partitioning]]
Weakness:
	- [[Internal vs External Fragmentation|External frag]]