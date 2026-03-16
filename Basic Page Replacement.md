4 Steps:
	1. Find the location of the desired page on disk
	2. Find [[Free Frame|free frame]]:
		- If there is, use it
		- else, use a [[Page Replacement Algorithm]] to select a victim frame
			- Write it to disk if ***dirty (has been modified after loaded)***
	3. Bring the desired pg to the new ff; update the pg and frame table
	4. Continue the proc by [[Instruction restart|restarting the ins ]]that caused the trap.

- Note: now potentially 2 page transfer for [[page fault]] - increasing #EAT 

![[Pasted image 20260314214219.png|532]]