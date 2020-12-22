# Code 401 | Socket.io

## Class 12 Reading Notes

I. Questions

- What is the benefit of transforming data into packets?: Because they are discrete units of data, they are ideal for being sent over a connectionless network that doesn't depend on nodes being connected one to another, making them dynamic and replaceable. [Indiana University](https://kb.iu.edu/d/anyq)

- Why is UDP often referred to as a connectionless protocol?: "There is no handshaking required before sending a message" [educative.io](https://www.educative.io/edpresso/what-is-udp), meaning that no connection need be established prior to the transmission of data [sciencedirect.com](https://www.sciencedirect.com/topics/computer-science/connectionless-protocol#:~:text=DNS%2C%20TFTP%2C%20and%20many%20other,the%20payload%20is%20not%20corrupted.)

- Can a socket-server application have multiple socket connections?:

- Can a socket-connection application be connected to multiple socket servers?:

- Can an application be both a socket server and a socket connection?: Yes, if you use two different ports or the sockets won't function simultaneously.

II. Vocabulary

- Observer Pattern

- Listener: likely refers to an event listener, used in JS to trigger a callback function once the event is "heard."

- Event Handler: a callback function that does something once an event is "heard" by the above listener.

- Event-Driven Programming: design and architecture of software with events as the guiding and driving principle.

- Event Loop: in general, the event loop refers, in JS, to the order of operations upon which it is based, with one thing necessarily being executed before another thing can begin. Per MDN, "JavaScript has a concurrency model based on an event loop, which is responsible for executing the code, collecting and processing events, and executing queued sub-tasks. This model is quite different from models in other languages like C and Java" [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop).

- Event Queue: "A JavaScript runtime uses a message queue, which is a list of messages to be processed. Each message has an associated function which gets called in order to handle the message. At some point during the event loop, the runtime starts handling the messages on the queue, starting with the oldest one. To do so, the message is removed from the queue and its corresponding function is called with the message as an input parameter. As always, calling a function creates a new stack frame for that function's use. The processing of functions continues until the stack is once again empty. Then, the event loop will process the next message in the queue (if there is one)" [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop).

- Call Stack: "A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc." [MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack).

- Emit/Raise/Trigger: terms used to describe the action of signaling that an event has occurred, so that a callback may be initiated.

- Subscribe: the term used to describe the relationship of an event listener to an event--it is said to subscribe to an event that it's listening to.

- database: "A structured set of data held in a computer, especially one that is accessible in various ways" (Oxford Languages via Google).

III. Preview



[<--back](401week1.md)

[<--home-->](../../README.md)
