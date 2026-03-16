- Seek time is the reason for differences in performance
- For a single disk there will be a number of IO request
- If requests are selected randomly, we will have poor performance.

#### Types of Polices
	 Ex Order of disk request: 55, 58, 39, 18,90 160,150,38,184
1. FIFO
	- Process request sequentially
	- Fair to all proc
	- Approaches random scheduling in perf if there are many proc
	 ![[Pasted image 20260315235202.png|572]]
2. Priority
	- Goal is not to optimize desk use but to meet other objectives.
	- Short batch jobs may have higher priority
	- Provide good interactive response time.
3. Shortest Service Time First *SSTF*
	- Select the disk IO request that require the least movement of the disk arm from its current position
	- ***Always choose the minimum Seek time***
	 ![[Pasted image 20260315214315.png|485]]
	 **Ex: if current position of disk arm is at track no. 100: then the first order would be 90
		 Full seq: 100,90,58,55,39,38,18,150,160,184 -> avg seek time (summation of difference)
4. SCAN (Elevator algo)
	- Arm moves in one direction only, satisfying all outstanding requests until it reaches the last track in that direction
	- *Direction is reversed*
	![[Pasted image 20260315214437.png|499]]
	**Ex: if current position of disk arm is at track no. 100:
		 Full seq: 100,150,160,184,90,58,55,39,38,
5. C-SCAN
	- Restricts Scanning to one direction only
	- When the last track has been visited in one direction, the arm is returned to the opposite end of the disk and the scan begins again
	- **Ex: if current position of disk arm is at track no. 100:
		 Full seq: 100,150,160,184,(return to 0 or lowest track num),18,38,39,55,58
	![[Pasted image 20260315215401.png]]
- Benchmark
 ![[Pasted image 20260315215421.png]]
