# Socket.io

[Web Sockets](https://en.wikipedia.org/wiki/WebSocket)


### What is a Web Socket?

WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

note that the Transmission Control Protocol (TCP) is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol (IP).

The WebSocket protocol enables interaction between a web browser (or other client application) and a web server. 
This is made possible by providing a standardized way for the server to send content to the client **without being first requested by the client**


### Describe the Web Socket request/response handshake and what happens once the connection is established.

To establish a WebSocket connection, the client sends a WebSocket handshake request, for which the server returns a WebSocket handshake response.

The handshake starts with an HTTP request/response **(it is like a formal conversation between two,They take turns speaking and listening)**, allowing servers to handle HTTP connections as well as WebSocket connections on the same port. Once the connection is established, communication switches to a bidirectional binary protocol **(WebSocket is like a more flexible and dynamic way of talking, means you can speak and listen to the other while speaking)**which does not conform to the HTTP protocol.

### Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client
without recieving a request from the client

## [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)



### What does the event handler io.on() do?

io.on() is a method provided by Socket.IO that allows you to listen for and handle different events that occur during the communication between the server and clients

### Describe some possible proof of life or proof that the code works as expected

Connection Establishment: Socket.IO relies on establishing connections between clients (such as web browsers) and the server. A proof of life can be shown by successfully establishing a connection between the client and the server using Socket.IO.#

### What does socket.emit() do?


The socket.emit() function is used in Socket.IO to send a custom event from the client (such as a web browser) to the server or from the server to a specific client. It allows you to send data or trigger events between the client and server in real-time.

## [Socket.io vs Web Sockets](https://www.educba.com/my-courses/learning/)



### What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).
|WebSocket|socket.io|
|-|-|
|1-WebSocket is a communication protocol that provides full-duplex communication channels over a single TCP connection. It enables real-time, bidirectional communication between a client (such as a web browser) and a server.|Socket.IO, on the other hand, is a library (or framework) that utilizes WebSocket as one of its transport mechanisms. It abstracts away the complexities of WebSocket and provides additional features to simplify real-time communication.|
|WebSocket allows both the client and server to send messages to each other at any time, without needing to initiate a new HTTP request for every message. |Socket.IO goes beyond the WebSocket protocol by adding features like event-based communication, automatic reconnection handling, room-based messaging, and support for real-time messaging across multiple servers or processes.|

### When would you use Socket.IO?

1. Chat Applications: Socket.IO is widely used for building chat applications

1. Collaboration Tools: Socket.IO is useful for developing collaborative applications such as shared whiteboards,

1. Real-Time Dashboards: Socket.IO is suitable for creating real-time dashboards or monitoring systems that require immediate updates and data visualization.

1. Multiplayer Games: Socket.IO is commonly used for building multiplayer games that require real-time interactions between players. 

### When would you use WebSockets?

1. Real-Time Chat Applications 
1. Collaborative Editing Tools: WebSockets are well-suited for collaborative editing tools, where multiple users can work on the same document simultaneously. 

1. ive Feeds and Notifications:  where users receive instant updates about specific events or content changes. 

1. Multiplayer Online Games: WebSockets are widely used in multiplayer online games to facilitate real-time communication between players and the game server.

## [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)


### What are a couple of key takeaways from this video?

1. Layered Structure: The OSI model is organized into seven layers, each serving a specific purpose and responsible for handling different aspects of network communication. 

1. Hierarchical Communication: The OSI model follows a hierarchical approach where each layer communicates with its corresponding layer on another device across a network. 

1. Abstraction and Encapsulation: The OSI model promotes the concept of abstraction, where each layer performs specific functions without needing to know the implementation details of other layers. 

1. Troubleshooting and Network Analysis: The OSI model assists in troubleshooting network issues by providing a systematic approach to identify and isolate problems. 


## [TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)

### Translate the gist of this video to a non-technical friend

Imagine you and your friend want to have a conversation using walkie-talkies. Before you can start talking, you both need to make sure that you can hear each other clearly. The TCP three-way handshake is a similar process that two computers go through to establish a reliable connection before they can start exchanging data.