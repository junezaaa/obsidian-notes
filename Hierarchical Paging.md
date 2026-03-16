#pgtablestruct 
- Break up the logical addr space into multiple page table with different hierarchies
- Called two-level page table.

#### Two-level Paging Example:
• Assume on a 32-bit address machine with 4KB page size
• A 32-bit logical address is divided into:
	– a page number consisting of 20 bits
		• Total number of pages is 2^20
	– a page offset consisting of 12 bits - ***To address every byte within a single page, you need exactly 12 bits.***

• Since the page table is paged, the page number is further divided into:
	– a 10-bit page number
		• Number of pages in the outer level is 2^10
	– a 10-bit page offset
		• Number of page tables of the inner level is 2^10

[[Address Translation Scheme|Address Translation Scheme of hierarchical pging]]
![[Pasted image 20260314013246.png]]
	Where pt_1 is an index to the outer page table, and pt_2 is the displacement within the page of the inner page table

## Two-level pg table demonstration
![[Pasted image 20260314013441.png|590]]