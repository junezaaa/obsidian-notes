Used by only one process at a time and will not be destroyed after used. Instead, it will release for reuse by other processes.

**Example of Reusable Resource :** Processor, I/O channels, RAM , Disk, semaphore.

[[Deadlock]] will occurs if each process holds one resource and requests the other.

**Example of Deadlock:** 

- P and Q competing for reusable resources D and T.
![[Pasted image 20260225140716.png]]
Then , p1 and q1 lock both D and T, so when the request D and T, they will blocked waiting for each other, causing [[Deadlock Condition#^c98ad5|circular wait]].
