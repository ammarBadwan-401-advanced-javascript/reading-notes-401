# Message Queues

## Message Queues

* A queue server runs independently and is tasked with routing events and messaging between clients.

* Any connected client can publish a message, any connected client can subscribe to recieve a message.

* The queue server can see which clients are connected and which queues they are attached to and subscribed to.

* Queue server recieves any published message and distributes it to all connected and subscribed clients.

* It ensures that subscribed clients can catch up and pull down any messages that they might have missed when they were disconnected.

## What is a message

* A message is a package of information thats categorized by queue and event.

1- Queue: which bucket does this belong to? ex: database events...

2- Event: Whats the occured event? ex: delete,add,error....

3- Payload: the data itself, like the id and text.

## Real Time vs Qeueud Messaging

* Real time messaging system are processed and broadcasted immediately to subscribers, if a connection is lost that client won't recieve anything.

* A queue will keep track of the delivery status of messages, any broadcast that isn't recieved will stay in the queue until it can be delivered.

### Use cases

1- API server responding to a POST request.

2- Logging applications

3- Web based dashboard.
