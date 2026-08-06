- HTTP request message
	- two types of HTTP msg: request, response
	- HTTP request msg: ASCII (human-readable format)
#Bookmark


- POST Method:
	- [[webpage]] often includes from input
	- user input sent from client to server in entity body of HTTP POST request message
- GET Method (for sending data to server):
	-  include user data in URL field of HTTP GET request msg (following a '?')
	- www.example.com/search?apple
- HEAD Method 
	- request header (only) that would be returned if specified URL were requested with an HTTP GET method
- PUT Method
	- uploads new file (object) to server
	- completely replaces file that exists at specified URL with content in entity body of POST HTTP request message