Reason for buffering 
	- Proc must wait for io to complete before proceeding
	- Certain pages must remain in main mem during io

- Block-oriented
	- Info is store in fixed sized block
	- Used for disk
- Stream-oriented
	- Transfer info as a stream of bytes
	- For terminals, printer, mouse, and most other devices that are not secondary storage

- Single Buffer
	- Block-ori
		- User proc can proc one block of data while next block is read in
		- Swapping can occur since input is taking place in sys mem, not user mem
		- OS keeps track of assignment of sys buffer to user proc
	- Stream-ori
		- Used a line at time
		- Output to the terminal is one line at a time
	- Circular Buffer
		- More than two buffers are used
		- Each individual buffer is one unit in a circular buffer
		- Used when io op must keep up with proc