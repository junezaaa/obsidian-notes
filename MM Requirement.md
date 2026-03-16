**Multiprogramming subdividing memory** needs to be allocated to ensure a reasonable supply of ready processes to consume available processor time.

MM intends to satisfy the following requirements:

1. **Relocation
	- Since programmer doesn't know where the program could be when executed, it could even be [[Swapping|swapped]] to a different location.
	- ***So memory reference must be translated in the code to actual physical memory address.***
2. **Protection
	- Must be satisfied by the hardware rather than the software (OS) to avoid overhead of sending it since OS cant anticipate all of the mem ref the program will make.
	- Each process should be protected against unwanted interference by other process, accident or not.
3. **Sharing
	- Any protection mechanism must have the flexibility to allow several processes to access the same portion of memory.
	- Better than to have their own separate copy, because its more efficient.
4. **Logical Organization
	- Programs that are organized into modules also provide sharing modules level among proc.
		- Which have its own degree of protection.
		- All references from one module to another resolved by the system at run time.
5. **Physical Organization
	- Two levels : Main mem and sec mem with its own purpose.
	- The flow of [[Swapping|swapping]] info between two levels should be a sys responsibility. 

