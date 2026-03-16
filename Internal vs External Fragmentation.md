- **Internal fragmentation** : If A doesn't use this leftover part, B also cant fetched it either.
- **External Fragmentation** : If the gaps between A and B are too small, C can't fit even if the total space is enough.
	- Which is reduced by **compaction**:
		- Shuffle mem contents to place all free mem together in one large block.
		- Can be done only if relocation is [[Dynamic Partitioning|dynamic.]]
		- Involved I/O and must do I/O only into OS buffers. *(Write/Read)*

![[Pasted image 20260315153948.png|568]]