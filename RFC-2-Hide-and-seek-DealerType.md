Dealer based hide an seek
=====

The server, using a dealer socket , hides behind an unknown hot-spot ,ip and port.
It sends the secret as soon as it starts, even if no one is connected.
As soon as the secret is sent, the server dies immediately. 

The first client which successfully connects to the server will receive the initial message
(which represents the secret). 


#####Possible IP ranges
192.168.1.*
#####Possible Port ranges 
3000 - 7000



