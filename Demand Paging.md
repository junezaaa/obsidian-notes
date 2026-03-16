	Demand paging brings a page into memory only when it is needed

Aspect:
- Pure demand paging - start proc with no pg in mem.
	- OS sets ins pointer to first ins of proc, non-mem-resident -> [[Page Fault|page fault]]
	- Hardware support needed for pure dp.
		- Pg table with [[Memory Protection#^9e9113|present/absent bit]]
		- Disk (with [[Swapping|swap]] space)
		- [[Instruction restart]]
#### Address Translation and demanding paging
![[Pasted image 20260314205605.png|626]]

### 12 Stages in Demand Paging (Worst case)
1. Trap to OS
2. Save user reg and proc state
3. Determine that the interrupt was a pg fault
4. Check that the pg ref was legal and determine the loc of the pg on the disk
5. Issue a read from the disk to a [[Free Frame|free frame]]
6. While waiting alloc the CPU to some other user
7. Receive an interrupt from the disk I/O sys when I/O read is completed
8. Save ref and proc state for other user
9. Determine the interrupt was from the disk
10. Correct pg table and other tables to show page is now in mem
11. Wait for CPU to be allocated to this process again
12. Restore the user reg and proc state, and new pg table, then resume the interrupted ins.

### Performance of Demand Paging
- Three major activities
	- Service the interrupt - 100+ ins needed
	- Read the pg - Lots of time
	- Restart the proc - quick
- Page fault rate 0 <= p <= 1
	- If p = 0, no pg fault
	- if p =1, every ref is a fault
#EAT
- [[Translation Lookaside Buffer#^aedf73|EAT]] =![[Pasted image 20260317042016.png|609]]
	**Example:**
	 ![[Pasted image 20260314212119.png|589]]