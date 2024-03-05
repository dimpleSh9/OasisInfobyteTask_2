# OasisInfobyteTask_2
Chat Application 

It is a chat application in which users interact in real time. It follows basic Client-Server architecture.

In this program it contains two scripts:
1. Server
2. Client 

Server Script 
💠It contains 5 functions. In main() an object of socket is created, which will be used to bind the Clients to the Ports, server limits will be set and client handle thread will be run to keep listening to the Clients.
💠Client_handle() takes client as parameters and inside, it takes username input and append the active user list to keep a track of users and runs listen_for_message thread.
💠Listen_for_message() takes client and username as parameters and input of message and display to others using messageToAll()

Client Script
💠It contains 4 functions. main() includes object of socket class with same functionality. It communicates to server 
💠 Comunicate_to_server() takes client as parameter and username input and runs a thread for message listening from server 
💠listen_for_message_from_server() takes client and parameters and it keep receiving messages from the server.
💠To display the message to other users send_message_to_server() is used. It takes client as parameters and message input and send it to all users.
