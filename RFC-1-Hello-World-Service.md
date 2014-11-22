Hello World Service
====

We're using tcp on port 5556. 

The client will send Hello and the server will reply with Hello. 

The Server and Client must be two different processes.

We want to make the server port and ip address configurable from the command line.

# Discovery

When the client connects to a new network

Then it opens a pub socket and send a hello message to every ip address

The content of the message is

freek 192.168.1.3:5556

Where the client name is freek and the address of the client is 192.168.1.3:5556. You are expected to send a message back to that address with the name of your server.

After replying you need to stop the server.
