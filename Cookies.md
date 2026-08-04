	maintaining user/server state

- Recall : HTTP GET/response interaction is [[HTTP#^60c5bc|stateless]]
- no notion of multi-step exchanges of HTTP msg to complete a Web "transaction"
	- no need for client/server to track "state" of multi-step exchange
	- all HTTP requests are independent of each other
	- no need for client/server to "recover" from a partially-completed-but-never-completed transaction

- Websites and client browser use cookies to maintain some state between transactions
	- four components
		1. cookie header line of HTTP res msg
		2. cookie header line in the next HTTP req msg
		3. cookie file kept on user's host, managed by user's browser
		4. back-end database at Web site

Example: the "Remember Me thingie", saving ID value to identification
![[Pasted image 20260805015309.png|491]]


HTTP Cookies usage:
- auth
- shopping carts
- recommendations
- user session state (Web e-mail)

Challenge: How to keep state?
- at protocol endpoints: maintain state at sender/receiver over multiple transactions
- in msg : cookies in HTTP msg carry state

- third party persistent cookie or tracking cookie are tracked across multiple web stie 

Example : tracking a user's browsing behavior

![[Pasted image 20260805015758.png|607]]