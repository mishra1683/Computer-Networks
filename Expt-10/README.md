# ARP implementation using UDP

## Aim :-

To implement ARP using UDP

---

## Algorithm :-

- Include the necessary header files.
- Create a socket using socket function with family AF_INET, type as SOCK_DGRAM.
- Declare structures arpreq ( as NULL structure, if required) and sockaddr_in.
- Initialize server address to 0 using the bzero function.
- Assign the sin_family to AF_INET and sin_addr using inet_aton().
- Using the object of arpreq structure assign the name of the Network Device to the data
- member arp_dev like, arp_dev=”eth0”.
- Ping the required Client.
- Using the ioctl() we get the ARP cache entry for the given IP address.
- The output of the ioctl() function is stored in the sa_data[0] datamember of the arp_ha
- structure which is in turn a data member of structure arpreq.
- Print the hardware address of the given IP address on the output console.
