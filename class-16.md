# Event Driven Applications

* Everything is event driven, including humans, from reacting to light,to driving cars.

* Machines can be event driven aswell, like the self-driving cars.

* How to leverage this in a software application? 

1- Everything in JS is an object.

2- Actions in JS are mostly event driven, such as UI events, express routes, hooks and react.

* An example: Every time we interact on a webpage through its UI, an event happens, from a button click to a key press, these events are associated with a function.

* Event driven concepts: 
1- Event handler is a callback function.

2- Main Loops listens for event triggers and calls the handler for them.

## Emitting Events

* Node.js provides a module called EventEmitter, that allows us to get started incorporating event driven programming.

* We can use it by requiring that module and creating a new object.

* We can add events to anything we want, for example adding an event to alert us when a user joins a chat room by using the emit method within the EventEmitter module.