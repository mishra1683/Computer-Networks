# UDP Client Server Data Communication

## Aim :-

To implement a simple UDP Client-Server application, where the Client on establishing a connection with the server, sends a string to the Server. The Server reads the String and prints it.

---

## Algorithm :-

### UDP Server –

1. Create UDP socket.
2. Bind the socket to server address.
3. Wait until datagram packet arrives from client.
4. Process the datagram packet and send a reply to client.
5. Go back to Step 3.

### UDP Client –

1. Create UDP socket.
2. Send message to server.
3. Wait until response from server is received.
4. Process reply and go back to step 2, if necessary.
5. Close socket descriptor and exit.
