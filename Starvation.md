
Starvation is a problem where a **process waits indefinitely for resources**, because another process that may have higher priorities keep interrupting it.

How is it related to Deadlock:
	[[Deadlock]] is closely related to starvation since in dl, **process also** **waits indefinitely** for other process to release resource.
What's the different:
	Starvation always have a schedule that feeds the starving process. While deadlock, if once occurs, it cannot be resolved by any possible future schedule, you can only schedule it [[Deadlock Avoidance|to avoid]] it.