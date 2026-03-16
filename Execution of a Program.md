- All pieces of a proc do not need to be loaded in main mem during exe.
- OS brings into main mem a few pieces of the prog
- **Resident set** - portion of proc that is in main mem ^853e66
- An interrupt is generated when an addr is needed that is not in main mem. 

- Piece of process that contains the [[Logical vs Physical Address Space|logical addr]] is brought into main mem
	- OS issued a disk I/O read request
	- Another proc is dispatched to run while the disk I/O takes place
	- When the I/O finished will issue an interrupt which causes the OS to place the affected proc in the Ready state
