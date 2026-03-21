### Library
	- Goal : want a db for borrowing book service and thesis 
- detail of the info that data going to collect for book:
	- book_name
	- author_name (fk)
	- publisher_name
	- print_date
	- call number
	- ISBN (primary key)

- detail of the info for the thesis:
	- thesis name
	- author_name 
	- stu_id
	- major
	- defense_year
	- advisor name
	- abstract
	- thesis call number

- for the borrowing service, student or teacher must register as a member of the library 
	- which collect the following:
		- mem_id
		- name
		- major
		- address
		- phone_num
		- email

- when borrwoing a service or thesis there will be borrow date and due date, and when the member succsefully return a book that borrow date and duedate will be rm from db


- Analysis of the demand: 
	- use bottom-up for the er design 
		- Bottom-up step by step
			- List all attribute
			- Normalize from 1nf to 3nf one at a time
		- Top-down step by step
			- Adding aggre relation ship along with entites
				- ![[Pasted image 20260319160320.png|441]]
			- Adding generalizion along with more specific entires
				- ![[Pasted image 20260319160332.png|423]]
			- Adding attr, prim key , connectively(t,e)
				- ![[Pasted image 20260319160437.png|436]]
	- ER model before modification
	- ![[Pasted image 20260319154328.png|592]]
	- After Modification ![[Pasted image 20260319155040.png]]

