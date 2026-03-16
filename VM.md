## Motivation:
- Combined size of the prog, data, stack **exceed** the amount of [[Logical vs Physical Address Space|physical mem]] available
- Code needs to be in memory to execute, but entire program rarely used; entire program code not needed at the same time.
## Virtual mem:
- ***Keep only portions of prog currently needed for exe in the mem and keep the rest on disk.***
- Can use Disk as though it were part of the main mem.
- Size of the virtual storage is limited by the addressing scheme and by the amount of sec mem, not by size of main mem.
	- Logical Addr space can therefore be **much large**r than physical addr space 
- Each prog takes less RAM while running
	- [[Degree of multiprogramming|More prog running concurrently]]
	- More CPU util
	- Less I/O needed to load or swap proc (since you only needed the necessary part)