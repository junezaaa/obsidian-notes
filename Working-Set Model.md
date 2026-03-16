#pr-algo 

	$ ≡ working-set window ≡ a fixed number of page ref
**Example**: 10000 Instructions
- WSSi (working set of proc Pi) = total number of pg ref in the most recent $ (varies in time)
	- If $ is too small will not encompass entire [[Principle of Locality#^6dc969|locality]] (high pg fault)
	- if $ is too large will encompass several localities (wasting memory)
	- If $ is infinite will encompass entire program
- D = ΣWSSi ≡ total demand frames -> approximation of locality
- If D > m -> [[Thrashing]] (*m is the number of available frame)
- Policy if D > m then suspend or [[Swapping|swap]] out one of the process 
- Prevent thrashing.

### Working sets and page fault rates
- The working set of a process changes over time as ref to data and code section move from one locality to another
- Assume no thrashing, the page-fault rate of the process will transition between peaks and valley overtime.

![[Pasted image 20260315143224.png|569]]