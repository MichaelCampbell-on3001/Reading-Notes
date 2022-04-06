# Message Queues

## [Socket.io [1] Chat Example](https://socket.io/get-started/chat/)

Check out a working example on your machine:

`git clone https://github.com/socketio/chat-example.git`

A simple chat app using Socket.io can be borken done into these steps:

- Serving HTML
- Integrating Socket.IO
- Emitting events
- Broadcasting

[1^] **Socket.IO** is composed of two parts:
- A server that integrates with (or mounts on) the Node.JS HTTP Server socket.io
- A client library that loads on the browser side socket.io-client


## [Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)
## Page Not Found, but below are links to rooms and namespaces:

[Rooms](https://socket.io/docs/v4/rooms/): A room is an **arbitrary channel** that sockets can **join and leave**. You can call **join** to **subscribe** the socket to a given channel. Upon **disconnection**, sockets **leave** all the channels they were part of **automatically**.

[Namespaces](https://socket.io/docs/v4/Namespaces/):  A **communication channel** that allows you to **split** the **logic** of your application.

**Every Namespace** has:
- Event handlers
- Rooms
- Middlewares

## [Socket.io Emit Cheatsheet](https://socket.io/docs/v3/emit-cheatsheet/) *The link provided didn't work for me so I found one that did and provided it here.*

### 3 Random Server-Side Cheats

 - To all clients in the current namespace except the sender:
  `socket.broadcast.emit(/* ... */);`
  - To all connected clients
  `io.emit(/* ... */);`
  - To individual socketid aka: a *private message*
  `io.to(socketId).emit(/* ... */);`


### 3 Random Client-Side Cheats

- With acknowledgement:
`socket.emit("question", (answer) => {
  ...
});`

- Without compression
`socket.compress(false).emit(/* ... */);`

- For a message that might be dropped if the low-level transport is not writable:
`socket.volatile.emit(/* ... */);`





