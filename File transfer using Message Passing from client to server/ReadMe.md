# File transfer using Message Passing from client to server

* This project aims to perform file transfer between clients and servers using static ports. 
* The file transfer happens in a byte stream by obeying certain restrictions applied on the file name and file size. 

# Servers
* The servers are programmed to receive files by multiple clients at the same time. 
* The server also enforces restrictions on the client’s file name size and the file size by itself. 
* The server is programmed to reject any files not complying with the above-mentioned restrictions.

# Client
* Each client sends a file to one server and stops after sending one file.
* While the server ports are static, client ports are dynamic since any client can transfer files to a specific server. 
* For the server to be able to identify the client correctly to acknowledge the message, the client packages its own port along with the message to be sent to the server. 
This way, the server unpacks the message along with the client port number and appropriately replies to the right client.

