# Sockets.io

__What is the benefit of transforming data into packets?__  
This is an efficient way of transfering data over networks and it limits latency.  
 
__UDP is often refereed to as a connectionless protocol. Why is this?__  
This is because with UPD no connection needs to be established between the origin and destination before tranferring data.  
 
__Can a socket server application have multiple socket connections?__  
Yes, a socket server can have more than one socket connection. We did this during our lab.  
__Can a socket connection application be connected to multiple socket servers?__  
I do not believe so. Each socket is bound to a single port.  
  
__Can an application be both a socket server and a socket connection?__   
It seems that a socket is mostly used to connect to a socket server, and not to be a server itself. However, I don't see why you could not have both in the same application.  
 


|Term | Definition |  
|---|---|
| OSI Model | OSI stands for Open System Interconnection. It is a conceptual framework for understanding the networking process. The seven layers of OSI are Physical, Data Link, Network, Transport, Session, Presentation, and Application.  |
| TCP Model | This is a more concise version of the OSI Model, and it consists of four layers: Application, Transport, Internet, and Network.|
|TCP | This stands for Transmission Control Protocol. In this, the server must be listening for connections from clients.  |
|UDP | This stands for User Datagram Protocol. Unlike TCP, there is no need to establish a connection before transfering data.  |
| Packets | A unit of data that goes from one place to another over a network.|
| Socket | A socket is an endpoint for sending and receiving data. Sometimes this refers to an internet socket, where a socket is identified to other hosts by its socket address.|