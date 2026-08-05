	to satisfy client requests without involving origin server

- Browser sends all HTTP requests to cache
	- if obj in cache : cache returns obj to client
	- else cache request obj from origins server, caches received obj, then returns obj to client

- Web cache acts as both client and server
	- server for original requesting client
	- client to origin server
- server tells cache about obj's allowable caching in response header

- *Why* Web caching?
	- reduce response time for client request
		- cache is closer to client
	- reduce traffic on an institution's access link
	- Internet is dense with caches
		-  enables "poor" content providers to more effectively deliver content

- Example #Bookmark
	- Problem 1 : At high access link utilization, the delay is very high if the access link rate is slow
		- Option 1 : buy a faster access link, but expensive
		- Option 2 : Install a Web cache