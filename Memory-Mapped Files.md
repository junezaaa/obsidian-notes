	 Mapping a file i/o contents (disk block) directly into page in memory.

- Initially read using [[Demand Paging]]
	-file is read from the file sys into physical page
- Speedup files acc by driving files i/o though mem rather than read() and write() sys call
- Also allows several procs to map the same file allowing the pages in mem to be [[Shared Page|shared]]
- The written data make it back to disk periodically , or/and at file close() time

![[Pasted image 20260315154819.png|408]]