#mmtech 
- Variable-partition sizes.
- Each proc is loaded into a partition of exactly the same size as that proc.
- [[Degree of multiprogramming]] are limited by number of partitions.
- Block of available memory, or [[Dynamic Storage Allocation|hole]], are various in sizes.
- When a proc arrive, it is allocated to a hole large enough to accommodate it.
**Strength** :
	- No [[Internal vs External Fragmentation|internal fragment]]
	- More efficient use of main mem.
Weakness:
	-Inefficient of processor use due to the need for [[Internal vs External Fragmentation|compaction]] to counter [[Internal vs External Fragmentation|external fragmentation]]
	
![[Pasted image 20260313155912.png|564]]
![[Pasted image 20260313155628.png|276]]