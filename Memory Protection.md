- Implemented by associating protection bit with each frame to indicate if ***W/R/X*** access is allowed.

- Present-absent bit attached to each entry in the [[Paging System|page table]] ^9e9113
	- "Present" indicates that the associated page is in the process logical addr spc, and thus a legal page
	- "Absent" indicates that the pg is not in the proc [[VM Key terms#^7ad3e6|logical addr spc]]
- Any violation result in a trap to the kernel