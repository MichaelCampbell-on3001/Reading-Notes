# Event Driven Applications

## [Event Driven Programming](https://alligator.io/nodejs/event-driven-programming/)

Anytime a user  **interacts** with a feature on an app such as clicking a button, navigating pages, following links an **event** occurs.

To achieve **event-driven progrgraming** a developer can follow these concepts.

- An Event Handler is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

**Node.js** provides a useful module called **EventEmitter** that allows a dev to incorporate Event-Driven Programming in a project quickly.

### Steps to use EventEmitter
1. the EventEmitter class can be found through the events module. Once a dev has imported the proper dependencies they are then able to create a new object from the class.

`const EventEmitter = require('events').EventEmitter;`

`const myEventEmitter = new EventEmitter;`

2. The scenerio bfor the code below is that if you wanted to create an event in a chatroom to alert users when a new person has entered the chat. 

`const EventEmitter = require('events').EventEmitter;`

`const chatRoomEvents = new EventEmitter;`

`function userJoined(username){`

`// Assuming we already have a function to alert all users.`

`alertAllUsers('User ' + username + ' has joined the chat.');`

`}`

`// Run the userJoined function when a 'userJoined' event is triggered.`

`chatRoomEvents.on('userJoined', userJoined);`

3. Finally use the **emit** method to trigger the event. Make sure to trigger it at within a login function inside the chatroom module.

`function login(username){`
`chatRoomEvents.emit('userJoined', username);`
`}`

**Note**: expansions on this idea include creating events for when users do other things like loggin out, sending a message and when that message is received or any other thign one might have seen in a chatroom before. 

**Object Oriented Programming + Event-Driven Programming**

Typically in programing, information flows one way, but by registering event listeners a developer can actually **reverse** the flow of communication between their objects. By doing this a dev's **objects** can just **emit events** and whichever objects are **listening** to those event will **process** it in the way they have been told to.

--- 


## [Node docs: events](https://nodejs.org/api/events.html)

### 5 Methods from the Node docs

- `emitter.eventNames()` - Returns an array listing the events for which the emitter has registered listeners. 

- `eventTarget.addEventListener(type, listener[, options])` - Adds a new handler for the type event. Any given listener is added only once per type and per capture option value.

- `event.preventDefault()` - Sets the defaultPrevented property to true if cancelable is true.

- `event.stopImmediatePropagation()` - Stops the invocation of event listeners after the current one completes.

- `eventemitterasyncresource.emitDestroy()` - **Call all destroy hooks.** This should **only ever be called once**. This must be **manually called**. 




