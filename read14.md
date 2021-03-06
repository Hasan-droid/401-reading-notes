# Event Driven Application

## Review, Research, and Discussion


- Complete file does not have to be downloaded in order to receive output.
- User can immediately start viewing data even though the complete file has not been transferred over. (Streaming services)
- UDP does not require a virtural circut to be established before any data transfer occurs
- a single port can accept 1 or more connections simultaneously
- The connections would be distinguished by a new variable with a different port or port endpoint

## Terminology

- Observer Pattern:
  - Design pattern used for one-to-many relationships
  - if one object is modified, its dependent relationships are mentioned automatically

- Listener:
  - a code block that is activated by a trigger

- Event Handler:
  - block of code (typically a callback) that is ran when the event is called upon

- Event Driven Programming:
  - programming paradigm where flow of program is determined by events/actions that trigger correlating code

- Event Loop:
  - monitors call stack and call back queue
  - if call stack is empty, event loop will take the first event from the queue and will push it to the callstack

- Event Queue:
  - design pattern of a queue of events awaiting to be processed by a program

- Call Stack:
  - a collection of code to be ran
  - FILO pushes and pops items off a stack

- Emit/Raise/Trigger:
  - an alarm that when alarmed will actiave/run corresponding code

- Subscribe:
  - an instance when a person/program decides to make a connection to pass each other data

- Database:
  - a structured collection of data that can be accessed, modified, and managed


## Preview

1. Which 3 things had you heard about previously and now have better clarity on?

- Event Driven Programming, Call Stack, Sockets

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- The complexities of Socket Io and other uses, Building a chat between 2 people, building a fully operation all that renders and updates information realtime

3. What are you most excited about trying to implement or see how it works?

- Rendering and updating apps in real time

## SNS vs SQS 

### SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

### SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll or pull messages from SQS. 

#### Messages can't be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. 

## References

- https://searchnetworking.techtarget.com/definition/UDP-User-Datagram-Protocol#:~:text=UDP%20(User%20Datagram%20Protocol)%20is,provided%20by%20the%20receiving%20party.
- https://en.wikipedia.org/wiki/Event-driven_programming