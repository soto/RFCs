Hide and seek protocol
====

There are nodes on the netwerk constantly publishing messages of the type: <ipaddress>:<port> via a ZMQ PublishSocket. If a seek client finds this server and then connects via a Request socket and sends a message with random content, the server will then shutdown.

The server is publishing on port 5556.