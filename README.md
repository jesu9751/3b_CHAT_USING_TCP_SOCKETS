# 3b.CREATION FOR CHAT USING TCP SOCKETS
## AIM
To write a python program for creating Chat using TCP Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server
4. Send and receive the message using the send function in socket.
## PROGRAM

## CLIENT 
```
import socket 
s=socket.socket() 
s.connect(('localhost',12345)) 
while True:
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
## SERVER
```
import socket 
s=socket.socket() 
s.connect(('localhost',12345)) 
while True:
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
## OUPUT
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/5a2945cd-1bbe-40ae-b542-ffba6d02c4ec" />

## RESULT
Thus, the python program for creating Chat using TCP Sockets Links was successfully 
created and executed.
