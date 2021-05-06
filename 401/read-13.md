# Message Queues


### What does it mean that web sockets are bidirectional? Why is this useful?
- It means that the socket can both send and recieve data a the same socket 
### Does socket.io use HTTP? Why?
- HTTP can be used in conjunction with HTTP and its does use it upon initial connection
### What happens when a client emits an event?
- that event gets published and is picked up by those set up to listen for it.
### What happens when a server emits an event?
- This will likely trigger functions in the subscribed clients
### What happens if a client “misses” an event?
- seems like its ignored although id hope thats not the answere
### How can we mitigate this?
- you could send confirmation events to confirm reception or throw errors.

# Terms
Socket - connection between browser and servers socket.
Web Socket - the name for the bi directional communication protocol.
Socket.io - JS lib for real time web apps
Client - user-side tx/rx software
Server - tx/rx for service side of apps
OSI Model - Open Systems Interconnection Model
TCP Model - Transmission Control Protocol, syn ack fin ack
TCP - package sending and recieveing
UDP - User Datagram Protocol
Packets - a data bundle that once send will be confiremd as recieved or re sent

### Which 3 things had you heard about previously and now have better clarity on?
- package sending
- sny, ack
- package loss
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- I am curious how async works with all this
- Redis adapters?
- creating and deleteing moves
### What are you most excited about trying to implement or see how it works?
- I would like to make a chat app like the tutorials I saw