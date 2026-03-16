4 times:
1. Proc creation
	- Determine prog size
	- create [[Paging System|pg table]]
2. Proc exe
	- [[MM Unit|MMU]] reset for new proc
	- [[Translation Lookaside Buffer]] flushed
3. [[Page Fault]] time
	- Determine [[VM Key terms#^fab5cc|virtual addr]] causing fault
	- swap target page out , needed page in
4. Proc termination time
	 - release pg table, pages