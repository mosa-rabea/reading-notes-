# Web Socket :

* You will build a server that accepts a message that carries a user’s name.
* In response, the server will push a greeting into a queue to which the client is subscribed.


* WebSocket is a communications protocol for a persistent,

* bi-directional, full duplex TCP connection from a user’s web browser to a server.

* A WebSocket connection is initiated by sending a WebSocket handshake
* request from a browser’s HTTP connection to a server to upgrade the connection.
* Along with the upgrade request header, 
* the handshake request includes a 64-bit Sec-WebSocket-Key header.
* The server responds with a hash of the key in a Sec-Websocket-Auth header.
* This header exchange prevents a caching proxy from resending previous WebSocket exchanges.

* What is WebSocket and why it is important?

* WebSocket is a two-way computer communication protocol over a single TCP.
* Using WebSockets is a good way to handle high scale data transfers between server-clients.