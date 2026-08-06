	HTTP/2 goal is to decrease delay in multi-obj HTTP request

- HTTP1.1: introduced multiple, pipelined GETs over single TCP connection.
	- server response *in-order* (FCFS) to GET requests.
	- with FCFS, small obj may have to wait for transmission (head-of-line blocking)
	- loss recovery (retransmitting lost TCP segments) stalls obj transmission 
- HTTP/2 #Bookmark 
	- increased flexibility at server in sending obj to clients
	- methods, status codes, most header fields unchanged from HTTP 1.1
	- transmission order of requested obj based on client-specified obj priority
	- push unrequested obj to client
	- divide obj into frames, schedule frames to mitigate HOL blocking (FCFS)
- HTTP/2 to HTTP/3
	- HTTP/2 over single TCP connection means:
		- recovery from packet loss still stalls all obj transmissions
			- as in HTTP 1.1, browsers have incentive to open multiple parallel TCP connections to reduce stalling, increase overall throughput
	- no security over vanilla TCP connection
	- HTTP/3: adds security, per obj error- and congestion-control (more pipelining) over UDP