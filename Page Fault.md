	If there is a ref to a pg, first ref to that pg will trap to os, which is called page fault

**Steps:**
1. OS looks at another table to decide
	- Invalid ref -> abort
	- Just not in mem
2. Find [[Free Frame|free frame]]
3. Swap page into frame via scheduled disk operation
4. Reset tables to indicate page now in mem; set [[Memory Protection#^9e9113|present/absent bit]] to 1.
5. [[Instruction restart|Restart the instruction]] that caused the page fault

![[Pasted image 20260314210103.png|477]]