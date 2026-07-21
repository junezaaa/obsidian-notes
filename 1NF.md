	Making all the data in the cell have "Atomic value" or value that can no longer subdivde
- 1NF Conditions:
	- No repeating groups: all attribute must have only one value per row (single-values)
	- Must have prim key per row
	- All data in a col must have same the dtype


Before 1NF
![[Pasted image 20260319022837.png|228]]
After 1NF
![[Pasted image 20260319022857.png|205]]

- Problem with 1NF:
	- Insertion anomaly occurs when inserting a new record causes many data items to be dupe or violates entity integrity
		- Ex: If you add a new record where its doesnt have t
	- Modification anomaly: occur when mod a record cause subsequent modification in many other records
		- Ex: if you change something like Id you also have to update every single row where a record is in said id
	- Deletion anomaly occur when remove record causes undesired info loss

### Fix by transforming [[1NF]] to [[2NF]]