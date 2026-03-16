[[Page Fault]] handling 11 steps:
	1. Hardware traps to kernel
	2. General registers saved
	3. OS determines which virtual page needed
	4. OS checks validity of address, seeks page frame
	5. If selected frame is dirty, write it to disk
	6. OS brings schedules new page in from disk
	7. Page tables updated
	8. [[Instruction restart|Faulting instruction backed up to when it began]]
	9. Faulting process scheduled
	10. Registers restored
	11. Program continues