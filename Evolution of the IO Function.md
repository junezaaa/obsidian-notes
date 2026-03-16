1. Proc directly control a peripheral device
2.  Controller or IO module is added
	- Procer uses prog IO without intercepts
	- Procer does not need to handle details of external devices
3.  Controller or IO module with interrupts
	- Procer doesnt need to spend time without waiting for IO operation to be performed
4. [[Direct Memory Access|DMA]]
	- Blocks of data are moved into memory without involving the procer
	- Procer involved at beginning and end only
5. IO module is a separate procer
	- Execute ins in main mem (IO channel)
6. IO procer
	- IO module has it own local mem
	- its a com with its own right
	- control sets of IO devices : comm , interactive terminals