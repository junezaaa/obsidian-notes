- A software counter associated with each page table entry, init zero
- Shift the counter right one bit before adding [[Not Recently Used Algorithm#^84028e|R bit]]
- R bit is added to the leftmost bit
- **Remove the page with the lowest counter**
- If refs occur at the same time, this algo cant tell the difference since it record one bit per time interval.

![[Pasted image 20260314230159.png|574]]