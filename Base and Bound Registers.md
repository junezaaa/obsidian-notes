	A pair of base and bound registers define the logical addr space

- Base register contains starting addr in memory of the process.
- Bound register indicates the ending location of the process

- CPU must check every **mem access generated** in the user mode to be sure if it is **between base and bound**. If it is, then proceed execution; else an interrupt is generated to OS.

![[Pasted image 20260313170136.png|629]]