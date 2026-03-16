
	TLB contain pg table entries that have been most recently used.

- Given a virtual addr, processor examines the TLB.
- **If TLB Hit**, via finding the [[Page Table Implementation#^e3be74|pg table entry]], the frame no. is retrieved, and the real addr is formed.
- **If TLB Miss**, the page num is used to index the proc pg table and get frame number from [[Address Translation Scheme|pg table]] in mem. Then a value is loaded into the TLB for faster access next time.
	- [[Page Replacement Algorithm|Replacement Policies]] must be considered
- TLB Lookup uses parallel search (One clock cycle search).

![[Pasted image 20260313181456.png|457]]

#EAT
**Effective Access Time (EAT)** : 
	TLB Lookup = ε time unit
		- Can be < 10% of mem acc time
	Hit ratio = α
	Miss ratio = 1- α
**(EAT formula)** :
	***= (Access#1 - ε) α + (Access#1+2 + ε) * ( 1 - α )***
Example: if α = 80%, ε = 20ns for TLB Search, 100ns for mem acc
	EAT = 0.8 x 120 *(from 100 + ε)* + 220 x 0.2 = **140ns** ^aedf73

TLB Table
![[Pasted image 20260314011416.png|384]]

**Use of TLB**
- First checks if page already in main mem
	- If not in there, issue a [[Page Fault|page fault]]
- TLB is updated to include the new page entry