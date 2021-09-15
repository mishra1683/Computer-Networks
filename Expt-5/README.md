# To print date and time using client-server communication

## Aim :-

To show Date and Time using a simple TCP Client-Server application.

---

## Algorithm :-

### Server -

1. Socket address structure
2. TCP/ UDF socket is created, an Internet socket address structure is filled with wildcard address & server's well known port
3. Bind function assigns a local protocol address to the socket
4. Listen function specifies the maximum number of connections that kernel should queue for this socket
5. The server to return the next completed connection from the front of the completed connection Queue calls it
6. Receiving the request message from the client

### TCP Client –

1. This function looks up a hostname and it returns a pointer to a hostent structure that contains all the IPV4 address
2. Socket address structure
3. Creating a socket, assigning IP address and port number for that socket
4. Connect establishes connection with the server using server IP address
5. Reads the message from standard input
6. Send function is used on client side to send data given by user on client side to the server
