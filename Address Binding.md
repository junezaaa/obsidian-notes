Process of mapping a [[Logical vs Physical Address Space|program logical addr to actual physical addr]] in the RAM.

Binding of instructions and data to memory addr can happen at three different stages:
- **Compile time**: Generate an **absolute code** if known where exactly the mem location for proc will be. Recompile if it changed.
- **Load time**:  Generate a relocatable code if mem location isn't known at compile time.
- **Execution time**: Addr Binding delayed until run time when reference is made to location in memory.
	- Require hardware support for addr maps [[Base and Bound Registers|(base and bound)]]