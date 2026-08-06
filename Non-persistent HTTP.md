- TCP connection opened to server
- multiple objects can be sent over single TCP connection between client and that server
- TCP connection closed
Example:
	- User enter URL www.someSchool.edu/someDepartment/home.index
	-
	1a. HTTP client init TCP connection to HTTP server at  www.someSchool.edu on port 80
		***I sent to server***
		***V***
	1b. HTTP server at host  www.someSchool.edu waiting for TCP connection at port 80 "accepts" connection, notifying client
		***I sent to host***
		***V***
	1. HTTP client send HTTP *request msg* (containing URL) into TCP connection socket. Msg indicates that client want object [someDepartment/home.index]
		***I sent to server***
		***V***
	2. HTTP server receives request message, forms response message containing requested object, and sends message into its socket
	3. HTTP server closes TCP connection
		***I sent to host***
		***V***
	4. HTTP client receives response msg contain html file, displays html. Parsing html file, find 10 refed jpeg obj
	5. **repeat step 1-5 for each of the 10 jpeg obj**
### Response time
- **RTT: time for a small packet to travel from client to server and back**
- HTTP res time (per obj) : 
	- One RTT to init TCP connection 
	- one RTT for HTTP req and first few bytes of HTTP res to return
	- obj/file transmission time
- So, response time is 2RTT = file transmission time
