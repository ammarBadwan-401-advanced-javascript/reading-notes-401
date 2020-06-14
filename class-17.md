# TCP Servers

## Event Queues

* A big part of NodeJS architecture is built around event usage, and every object that emits an event is an instance of EventEmitter constructor.

* EventEmitters are great at handling the controls of asynchronous events.

* Disconnected services can communicate with each other using proprietary API's, this is done throught a a central hub (or a queue) which recieves all messages.

## OSI Model

* Open Systems Interconnection Reference Model (OSI model) was developed in the mid 1980's as a seven layer model, it continues to describe the difference process in computer networking.

* It's still used as a point of reference while working in networked systems.

* These are the layers:

7- Application 

6- Presentation

5- Session

4- Transport

3- Network

2- Data Link

1- Physical

## Internet Protocol Suite

* IPS is often referred to as TCP/IP.

* IPS uses four layers: Link, Internet, Transport and Application layers.

### TCP

* Transmission Control Protocol (TCP) is a widely used application layer protocol in the IPS.

* It creates two way communication between the two hosts.

### TCP Header

* It controls the type of interaction being sent.

* It contains: 16 bit source port, 16 bit destination port, 32 bit sequence number, 32 bit acknowledgement numbeer, 4 it data offset and 9 bits flag.

* The flags are: `NS CWR ECE URG ACK PSH RST SYN FIN`, each with their own meanings.

* It also contains a 16 bit window size, 16 bit checksum, 16 bit urgent pointer (if URG is set) and a variable 0 to 320 bit options section.

### Connection Establishment

* Client sends SYN Packet with a random initial sequence number.

* Server sends SYN-ACK packet with acknowledgement number set to one more than the initial sequence number, then clien responds with ACK and AK number incremented by 1.

## Connection Termination

* One end sends a FIN segment and other sends an ACK segment then a FIN segment, termination initiation wil respond with ACK segment.