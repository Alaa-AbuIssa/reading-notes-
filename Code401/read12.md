# Sockets.io

**What is the benefit of transforming data into packets?**  
This is an efficient way of transfering data over networks and it limits latency.

**UDP is often refereed to as a connectionless protocol. Why is this?**  
This is because with UPD no connection needs to be established between the origin and destination before tranferring data.

**Can a socket server application have multiple socket connections?**  
Yes, a socket server can have more than one socket connection. We did this during our lab.  
**Can a socket connection application be connected to multiple socket servers?**  
I do not believe so. Each socket is bound to a single port.

**Can an application be both a socket server and a socket connection?**  
It seems that a socket is mostly used to connect to a socket server, and not to be a server itself. However, I don't see why you could not have both in the same application.

| Term      | Definition                                                                                                                                                                                                                      |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OSI Model | OSI stands for Open System Interconnection. It is a conceptual framework for understanding the networking process. The seven layers of OSI are Physical, Data Link, Network, Transport, Session, Presentation, and Application. |
| TCP Model | This is a more concise version of the OSI Model, and it consists of four layers: Application, Transport, Internet, and Network.                                                                                                 |
| TCP       | This stands for Transmission Control Protocol. In this, the server must be listening for connections from clients.                                                                                                              |
| UDP       | This stands for User Datagram Protocol. Unlike TCP, there is no need to establish a connection before transfering data.                                                                                                         |
| Packets   | A unit of data that goes from one place to another over a network.                                                                                                                                                              |
| Socket    | A socket is an endpoint for sending and receiving data. Sometimes this refers to an internet socket, where a socket is identified to other hosts by its socket address.                                                         |


## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
 ***event in node.js, emmiter***
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
***more about emmit methode***
3. What are you most excited about trying to implement or see how it works?
***the testing***


## Preparation Materials
* WebSocket : is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

* WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket “is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries,” thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header[1] to change from the HTTP protocol to the WebSocket protocol.

* Socket.IO enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket.IO is built on top of the WebSockets API (Client side) and Node.js. It is one of the most depended upon library on npm (Node Package Manager).

Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of:

* a Node.js server: Source	API
* a Javascript client library for the browser (which can be also run from Node.js): Source	API

```
const socket = new WebSocket("ws://localhost:3000");

socket.onopen = () => {
  socket.send("Hello!");
};

socket.onmessage = (data) => {
  console.log(data);
};
```