# Code 401 | Message Queues

## Class 13 Reading Notes

I. Questions

- What does it mean that web sockets are bidirectional? Why is this useful?: "Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time. In the context of networked AV and control systems, this allows devices to send and receive continuous streams of data to and from any point on the network" ([AMX](https://www.amx.com/en/site_elements/benefits-and-applications-of-websockets)). Put more plainly, this means that a server can push messages to a client without waiting for a request from a client.

- Does socket.io use HTTP? Why?: I understand that socket.io uses WebSocket and, in the event that the connection cannot be established, will resort to HTTP long-polling ([socket.io](https://socket.io/docs/v3/index.html). As such, the answer to this question seems to be yes.

- What happens when a client emits an event? It triggers the next server event.

- What happens when a server emits an event?: it generates a message that gets queued and, if the client is on, sent; or, if not, saved for delivery in the queue.

- What happens if a client “misses” an event?: it gets delivered, along with other missed messages, when the client logs back on.

- How can we mitigate this? Mitigate what, exactly? The client missing an event? Isn't that what the queue is for?

II. Vocabulary

- Socket: "A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. An endpoint is a combination of an IP address and a port number" ([Oracle](https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html#:~:text=Definition%3A,address%20and%20a%20port%20number.)).

- Web Socket: "WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. . . . WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with the HTTP protocol. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol" ([Wikipedia](https://en.wikipedia.org/wiki/WebSocket#:~:text=WebSocket%20is%20a%20computer%20communications,WebSocket%20is%20distinct%20from%20HTTP)).

- Socket.io: "Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of a Node.js server [and]
a Javascript client library for the browser (which can be also run from Node.js) [Socket.io](https://socket.io/docs/v3/index.html).

- Client: "A client is a computer or a program that, as part of its operation, relies on sending a request to another program or a computer hardware or software that accesses a service made available by a server (which may or may not be located on another computer)" ([Wikipedia](https://en.wikipedia.org/wiki/Client_(computing)#:~:text=A%20client%20is%20a%20computer,be%20located%20on%20another%20computer)). 

- Server: "a server is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients". This architecture is called the client–server model. Servers can provide various functionalities, often called "services", such as sharing data or resources among multiple clients, or performing computation for a client. A single server can serve multiple clients, and a single client can use multiple servers" [(Wikipedia)](https://en.wikipedia.org/wiki/Server_(computing)#:~:text=In%20computing%2C%20a%20server%20is,devices%2C%20called%20%22clients%22).

- OSI Model: Open Systems Interconnection Model, it is a "conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software. In the OSI reference model, the communications between a computing system are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application" [(forcepoint.com)](<https://www.forcepoint.com/cyber-edu/osi-model#:~:text=The%20OSI%20Model%20(Open%20Systems,between%20different%20products%20and%20software>).

- TCP Model: "TCP (Transmission Control Protocol) is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data. TCP works with the Internet Protocol (IP), which defines how computers send packets of data to each other" [(techtarget.com)](https://searchnetworking.techtarget.com/definition/TCP#:~:text=TCP%20(Transmission%20Control%20Protocol)%20is,of%20data%20to%20each%20other).

- UDP: "User Datagram Protocol (UDP) – a communications protocol that facilitates the exchange of messages between computing devices in a network. It’s an alternative to the transmission control protocol (TCP). In a network that uses the Internet Protocol (IP), it is sometimes referred to as UDP/IP. UDP divides messages into packets, called datagrams, which can then be forwarded by the devices in the network – switches, routers, security gateways – to the destination application/server. While UDP does not number or reassemble the datagrams, it does include port numbers in the datagram header that help distinguish different user requests and an optional checksum capability that can help verify the integrity of the data transferred" [(sdxcentral.com)](https://www.sdxcentral.com/resources/glossary/user-datagram-protocol-udp/#:~:text=User%20Datagram%20Protocol%20(UDP)%20%E2%80%93,referred%20to%20as%20UDP%2FIP).

- Packets: "A packet is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred" [(techterms.com)](https://techterms.com/definition/packet#:~:text=A%20packet%20is%20a%20small,(or%20data)%20being%20transferred).

III. Preview

A. Links for reading:

- [socket.io chat example](https://canvas.instructure.com/courses/2443160/discussion_topics/10234970)

- [Rooms and namespaces](https://socket.io/docs/v3/rooms/index.html)

- [socket.io emit cheatsheet](https://socket.io/docs/v3/emit-cheatsheet/index.html)

B. Reading Prompts

- Which 3 things had you heard about previously and now have better clarity on?
  - What it means that a socket is bidirectional.
  - That rooms and namespaces are a server-side thing, not a client-side one.
  - io.to and io.in are the same thing.

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- What are you most excited about trying to implement or see in action?: tying the server to a front end.

[<--back](401week3.md)

[<--home-->](../../README.md)
