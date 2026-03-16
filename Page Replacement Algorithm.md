#pr-algo
![[Pasted image 20260314214639.png]]

**Frame alloc algo determine:**
	- How many frames to give each proc
	- Which frames to replace ^9a48bf

**Pg replacement algo:**
	- ***Want lowest [[Page Fault|pg-fault]] rate***
	- Evaluate algo by running it on a particular string of mem ref
		- Ref str is just a pg num, not full addr
		- Repeated acc to the same pg does not cause a pg fault
		- Result depend on number of frames available
	![[Pasted image 20260314215200.png|424]]
***Type of page replacement algo:***
	1. [[Optimal Algorithm]]
	2. [[Not Recently Used Algorithm]]
	3. [[FIFO Algorithm]]
	4. [[Second Chance Algorithm]]
		4.1 [[Clock Algorithm]]
	5. [[Least Recently Used Algorithm]]
		5.1 [[LRU Not Frequently Used Algorithm]]
		5.2 [[LRU Aging algo]]
	6. [[Stack Algorithm]]
	7. [[Working-Set Model]]
		7.1 [[WS-Clock Algorithm]] ^6e66b2

Summary of Each Algo:

| Algoritm        | Comment                      |
| --------------- | ---------------------------- |
| 1.Optimal       | Benchmark                    |
| 2.NRU           | Very crude approx of LRU     |
| 3. FIFO         | Might throw out important pg |
| 4 Second chance | > FIFO                       |
| 5 LRU           | Great, but hard to implement |
| 6 NFU           | Fairly crude approx of LRU   |
| 7 Aging         | Approx LRU well, efficient   |
| 8 Working set   | Expensive to implement       |
| 9 WSClock       | Good effi algo               |

