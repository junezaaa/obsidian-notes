
-  Program must be brought from disk into memory and placed within a process to run
- Memory is just a linear sequence, or stream of bytes
- Main memory and registers are only storage CPU can access directly
- **Premise of MM**:
	1. Register access in <= one CPU clock
		While main memory can take many cycles, causing a ***stall*** on CPU
	2. Protection of memory required to ensure correct operation
	
	- *So the point of MM is to mainly manage both of these to make CPU have a high utilization.*