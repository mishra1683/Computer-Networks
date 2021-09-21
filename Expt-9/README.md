# Remote Command Execution using UDP

## Aim :-

Remote Command execution is implemented through this program using which Client is able to execute commands at the Server. Here, the Client sends the command to the Server for remote execution. The Server executes the command and the send result of the execution back to the Client.

---

## Algorithm :-

### Server -

1. Include the necessary header files.
2. Create a socket using socket function with family AF_INET, type as SOCK_DGRAM.
3. Initialize server address to 0 using the bzero function.
4. Assign the sin_family to AF_INET, sin_addr to INADDR_ANY, sin_port to dynamically assigned port number.
5. Bind the local host using the bind() system call.
6. Within an infinite loop, receive the command to be executed from the client.
7. Append text “> temp.txt” to the command.
8. Execute the command using the “system()” system call.
9. Send the result of execution to the Client using a file buffer.

### Client -

1. Include the necessary header files.
2. Create a socket using socket function with family AF_INET, type as SOCK_DGRAM.
3. Initialize server address to 0 using the bzero function.
4. Assign the sin_family to AF_INET.
5. Get the server IP address and the Port number from the console.
6. Using gethostbyname() function assign it to a hostent structure, and assign it to sin_addr of the server address structure.
7. Obtain the command to be executed in the server from the user.
8. Send the command to the server.
9. Receive the output from the server and print it on the console.
