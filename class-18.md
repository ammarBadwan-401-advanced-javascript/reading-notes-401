# Socket.io

## Web Sockets

* Its a communication protocol that provides bidirectional communications between server and client over TCP.

* WebSocket remains open all the time to allow real-time data transfer.

* After a request is triggered, the server doesn't close the connection, or vice versa.

## Socket.io

* A library that enables real time communications between client and web servers.

* It utilizes the WebSocket protocol to provided the interface.

* It's divided into two parts, both of them use WebSockets but also provides other functionalities such as broadcasting, namespacing and other means of grouping clients.

1- Client side: A library that runs in the browser.

2- Server side: A library that runs ins NodeJS.

## Connections

* TCP keeps the server connection alive.

* Socket.io you connect to server over HTTP, and its kept alive through its internal use of WebSocket protocol.

## Messaging

* Socket.io uses emit() and on() just like NodeJS.

* In nodejs, no external application can participate in the events present in the app itself.

* In socket.io, thepoint is to share events between disconnected participants throught a server, client connects, emits an event and respond to events from server, the flow goes like:

1- Client app #x connect to a running socket.io.

2- Client app emits event called speak to server.

3- Server has a listener for that event.

4- After processing the event, the server might: broadcast() or emit() an event, or the message might be sent to individual clients.

5- Other client application that are connected may have a listener for that event and can hear it aswell.

* Not all clients have listeners for every event, and vice versa.