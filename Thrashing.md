	Process is busy swapping pages in and out

- Since proc doesnt have enough pages the [[Page Fault]] rate is very high
	- Replace frame, but quickly need to get it back.
		- Low CPU util
		- OS thinks it need to increase [[Degree of multiprogramming]] , which is a bad idea because if even more proc need pg, then the demand will even be higher = more pg fault

![[Pasted image 20260315145743.png|414]]

#### Process suspension for thrashing avoidance
- Lowest priority proc
- Faulting proc
	- Does not have its [[Working-Set Model|ws]] in main mem so will be blocked anyway
- Last proc activated
	- This proc is least likely to have its working set [[Execution of a Program#^853e66|resident]]
- Proc with smallest resident set
	- Least effort to reload later in the line.
- Largest proc
	- Obtains the most free frames
- Proc with the largest remaining exe remain exe window (1%/100% ex)