***- [[VM|Virtual memory]] allow files and memory to be shared by two+ proc through page sharing.***

- **Shared code** 
	- One copy of read-only code are shared
	- Similar to threads sharing the same proc space
	- Also useful for IPC if sharing of read-write pg is allowed
- Private code and data:
	- Each pro keeps a separated copy of the code and data
	- the pg for them can appear any where in [[Logical vs Physical Address Space|logical addr space]]
![[Pasted image 20260314020028.png|405]]