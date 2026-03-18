	The property that attributes unquely indentifies other attributes is called functional dependency (FD)

- FD : given a relation R, a set of attributes B (called nondeterminant) is functionally dependent on another set of attributes A (determinant) if each A value is associated with only one B value, Such an FD is denoted by A -> B, in summary if you know value of A **(determinant)**, you can know the value of B **(nondeterminant)** ^2e4618
	- Ex : three attributes: `Student_ID`, `National_ID`, and `Student_Name`.
		- If i l know the student_id, then i will know the name of the student by looking for it
			- 'stu_id' -> stu_name
		- but if i only know stu_name i may find different ids with the same name since a determinant value can only led to a specific nondeterminant value

#### Goal of 2NF
	- ensure every non-key attr is fully  dependent on the prim key (Not composite)
	- it also must met 1NF requirement

Step by step
	- Eliminate partial dependency by breaking the table apart

- Problem with 2nf
	-Same with 1nf but less severe
	
Fix by transforming 2nf to [[3nf]]
from:
![[Pasted image 20260319030321.png|297]]
to:
![[Pasted image 20260319030329.png|697]]