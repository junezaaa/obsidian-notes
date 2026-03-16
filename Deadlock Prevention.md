Possible Sol for each [[Deadlock Condition]]
1. Mutex  - cant do shit
	- No rec ever assigned exclusively to a single proc - spooling
	- avoid assigning rec unless necessary
2. Hold and Wait
	- Must guarantee that when a proc req a rec, it doesnt hold any rec
	- require proc to req and alloc all its rec at one
	- require a proc reqing a rec to release all the rec it currently held
	- low rec util, [[starvation]]
3. No preempt
	- If proc that is holding rec req another rec that cannot be alloc immediately, it release the held rec, and has to req them again (risk for starvation)
4. Circular Wait
	1. linear ordering of all resource type, request a rec in a sequential ordering