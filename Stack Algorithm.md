	literally a down convery belt
	
#pr-algo 

- Array M is used to keep track of the state of mem, start empty
- When Top part is full, invoke a replacement algorithm and remove a page from the top part to the bottom part.
![[Pasted image 20260314231235.png|655]]

#### Property of the stack algo  (inclusion property)
 ![[Pasted image 20260314232705.png|271]]
***"Pages in the top part of r for memory with n pages frames after r memory refs are also in M more memory with m+1 page frames"***
- Meaning it doesn't suffer from [[FIFO Algorithm#^9068dd|Belady's Anomaly]]
