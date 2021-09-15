# Implementation of File Transfer Protocol

## Aim :-

To implement of File Transfer Protocol

---

## Algorithm :-

### Server -

1. Include the necessary header files.
2. Create a socket using socket function with family AF_INET, type as SOCK_STREAM.
3. Initialize server address to 0 using the bzero function.
4. Assign the sin_family to AF_INET, sin_addr to INADDR_ANY, sin_port to dynami cally
5. assigned port number.
6. Bind the local host address to socket using the bind function.
7. Listen on the socket for connection request from the client.
8. Accept connection request from the Client using accept function.
9. Within an infinite loop, receive the file name from the Client.
10. Open the file, read the file contents to a buffer and send the buffer to the Client.

### Client -

1. Include the necessary header files.
2. Create a socket using socket function with family AF_INET, type as SOCK_STREAM.
3. Initialize server address to 0 using the bzero function.
4. Assign the sin_family to AF_INET.
5. Get the server IP address and the Port number from the console.
6. Using gethostbyname function assign it to a hostent structure, and assign it to sin_addr of
7. the server address structure.
8. Within an infinite loop, send the name of the file to be viewed to the Server.
9. Receive the file contents, store it in a file and print it on the console.
