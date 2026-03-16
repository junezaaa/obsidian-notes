#pr-algo 

	Two status bits are associated with each page table entry
		- R bit is set whenever the page is ref
		- M bit is set when page is modified
	Upward Converyor belt

^84028e

- Bit is only reset util the OS resets it
- ***R bit is cleared every n clock interrupt , or R will be pointless since all R = 1***
- When pg fault occur, pg can be categorized in to 4 classes

![[Pasted image 20260314221858.png|650]]

	This algo prioritize removing class 0-1-2-3.
	
![[Pasted image 20260314222442.png]]
