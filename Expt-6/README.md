# Half Duplex Chat TCP/IP

## Aim :-

To implement half-duplex chat using a simple TCP Client-Server application

---

## Algorithm :-

### Server –

1.  Create the Server structure.
2.  Create TCP socket.
3.  Bind the socket to server address.
4.  Wait until message arrives from client.
5.  Process the message and send a reply to client.
6.  Go back to Step 3.

### Client –

1.  Create the socket.
2.  Send message to server.
3.  Receive data from the server, then print the data
4.  Process reply and go back to step 2, if necessary.
5.  Close socket descriptor and exit.
