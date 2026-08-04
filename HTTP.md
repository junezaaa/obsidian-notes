	hypertext transfer protocol

- Web's application-layer protocol
- client/server model:
	- client browser that request, receives, and displays Web objects
	- server: Web server sends (using HTTP protocol) objects in response to requests.

![[Pasted image 20260805005858.png|325]]


HTTP uses TCP:
- client initiates TCP connection (creates socket) to server, port 80
- server accept TCP connection from client
- HTTP msg (application-layer protocol msg) exchanged between browser (HTTP client) and Web server (HTTP server)
- TCP connection closed

HTTP is "stateless" ^60c5bc
- server maintain no info about past client request 
- state past history are complex anyway could be inconsistent also