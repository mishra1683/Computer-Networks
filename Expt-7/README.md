# Full Duplex Chat TCP/IP

## Aim :-

To implement full-duplex chat using a simple TCP Client-Server application.

---

## Algorithm :-

### Server -

1. Include the necessary header files
2. Create a socket using socket function with family AF_INET, type as SOCK_STREAM
3. Initialize server address to 0 using bzero function
4. Assign the sin_family to AF_INET, sin_addr to INADDR_ANY, sin_port to dynamically assigned port number
5. Bind the local host address to socket using the bind function
6. Listen on the socket for connection request from the client
7. Accept connection request from the client using accept function
8. Fork the process to receive message from the client and print it on the console
9. Read message from the console and send it to the client

### Client -

1. Include the necessary header files
2. Create a socket using socket function with family AF_INET, type as SOCK_STREAM
3. Initialize server address to 0 using bzero function
4. Assign the sin_family to AF_INET
5. Get the server IP address and the Port number from the console
6. Using gethostbyname function assign it to a hostent structure, and assign it to sin_addr of the server address structure
7. Request a connection from the server using the connect function
8. Fork the process to recieve message from the server and print it on the console
9. Read message from the console and send it to the server
