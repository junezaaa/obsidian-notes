
#### Non-Persistent HTTP issues:
- 2 RTTs per obj
- OS overhead for each TCP connection
#### **Persistent HTTP (HTTP 1.1)**
- server leaves connection open after sending response
- subsequent HTTP msg between same client/server sent over open connection
- client sends requests as soon as it encounters a ref obj
- as little as one RTT for all the ref obj (cutting res time in half)

