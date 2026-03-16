#mmtech 
***- Premise of paging***
	**Main memory** is divided into a number of equal-size **frame. (Physical mem)**
	**Each process** is divided into a number of equal-size **pages (Logical mem)** of the same length as frames. ^668812

- A process is loaded by **loading all of its page** into available, not necessarily contiguous frames.

Strength:
	- No [[Internal vs External Fragmentation|external frag]].
	- Avoid problem of varying sized mem chunks.
Weakness:
	- A small amount of [[Internal vs External Fragmentation|internal frag]], depending on *page size (Main issue)*.


![[Pasted image 20260313172311.png|655]]