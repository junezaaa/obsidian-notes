	4NF eliminates redundancy caused by multivalued dependencies by separating independent one-to-many relationships into different tables.

- Multi-valued dependence (MVD)
	- For X -> Y, for a single X , multiple values of Y exist

![[Pasted image 20260319040145.png|370]]
- Course ->-> Teacher
- Course ->-> Textbook

TO:
	![[Pasted image 20260319041240.png|518]]
***4NF may suffer from cyclic constraint***
	Where A depend on B which depend on C, and C circle back and depend on A