# Message Queues

**What does it mean that web sockets are bidirectional? Why is this useful?**  
Bidirectional means that both parties on either side of a network can experience the same thing simultaneously. This is in contrast to HTTP that will either do a request or a response.

**Does socket.io use HTTP? Why?**  
Socket.io uses the WebSocket Protocol instead of HTTP because it allows for real time data transfer.

**What happens when a client emits an event?**  
The server will listen for that event and react to it, and it will alert other clients if it is supposed to.

**What happens when a server emits an event?**  
All of the sockets/clients listening to the server will react to the event.

**What happens if a client “misses” an event?**  
This could seriously interupt the flow of an application where events rely on one another.  
**How can we mitigate this?**  
We need to use great error handling to catch there problems when they occur and to minimize the problems associated with a missed connection.

| Term       | Definition                                                                                                                                                         |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Web Socket | The communication protocol that allows a client and a server to connect over a TCP protocol. The Web Socket remains open to allow real time data transfer.         |
| Socket.io  | Socket.io broadcasts mulitple sockets at a time, and it works on all platforms. It also allows real time data transfer, and there are many advantages to Socket.io |
| Client     | This is what accesses a server to get information. The client is the one asking for information or data, and the server is providing it.                           |
| Server     | A server provides functionality, data, and information to clients. A single server can serve mulitple clients.                                                     |


## Preview:
1. Which 3 things had you heard about previously and now have better clarity on?
***Clients, Servers, and Socket.io***
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
***Socket.io,OSI and TCP***
3. What are you most excited about trying to implement or see how it works?
***Working with creating servers and clients and making them optimal!***