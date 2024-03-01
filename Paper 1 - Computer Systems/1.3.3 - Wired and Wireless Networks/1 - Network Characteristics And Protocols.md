
# What is a Network?

- We call a single computer, that is not connected to anything else a ***Standalone Machine
- Once you connect 2 Standalone Machines together, whether wired or wirelessly, you have a ***Network***

- Networks can come in many different sizes:
	-  Small business networks with a handful of devices
	- Large corporate networks with thousands of devices 
	- The largest network in the world, The Internet

## Packet and Circuit Switching

- ***Circuit Switching*** provides the basis for traditional phone networks
- This method creates a temporary link of fixed bandwidth between the source and destination that lasts until the transmission is complete
- This method guarantees the quality of the transmission, and is very reliable which makes it an excellent choice for real time video
- The downside is that a lot of potential bandwidth is wasted

# Protocols

- A protocol is basically just another word for a standard, it is a set of rules that we follow, so that every system communicates in the same way, ensuring that everything is compatible
- There are 9 protocols that we need to know for this course
	1) TCP
	2) IP
	3) UDP
	4) HTTP
	5) HTTPS
	6) FTP
	7) POP
	8) IMAP
	9) SMTP

## TCP/IP And UDP

- TCP, or Transmission Control Protocol, is a standard that enables programs/devices to exchange messages over a network.
	- It ensures the reliable transmission of packets using many techniques of checking whether the packets of data are valid.
	- E.g. Checksum, where the header of each packet is added up into a checksum, and if the received message's checksum is now different, we know that a packet has been lost along the way.

- UDP, or User Datagram Protocol, is a simple, connectionless transmission model.
	- It is an alternative to TCP, with no error checking
	- Mostly used for sending short messages using datagrams where speed is more important than accuracy

