# Data Communication
<hr>
### Protocol Data Units

Getting data from one end of the network to another relies on something called a PDU (Protocol Data Unit).

- Protocol Data Units are also known as "Transmission units" because we are taking some data and moving it across the network as a single unit
- Ethernet operates on a frame of data
	- It doesn't care whats inside of this frame
- IP operates on a packet of data
	- Inside is TCP or UDP but IP doesn't care
- Where there is a TCP or UDP header, there will be
	- A TCP segment
	- A UDP datagram
<hr>

### Encapsulation and Decapsulation
##### Encapsulation
![[002 encapsulation.png]]
##### How data encapsulation works?
1. We create Application Data at Layers 5, 6 & 7 (The Application Layers)
2. The Application Data gets enclosed within a TCP/UDP Header (The Transport Layer)
3. The TCP/UDP Header and Application data are enclosed within an IP Header (The Network Layer)
4. The IP Header, TCP/UDP Header & Application Data are enclosed within a Frame Header and Frame Trailer

<hr>

### Sending data across the network (Enapsulation & Decapsulation)
![[002 udpencapsulation.jpg]]

##### Decapsulation
1. When we send data to another computer on a network the data gets encapsulated first, and when the receiving computer gets the encapsulated data it must decapsulate the data. The process is as follows:
2. First the Frame Header and Frame Trailer get removed from the data
3. Then the IP Header gets removed from the data 
4. After the IP Header gets removed the TCP/UDP Header gets removed
5. Finally we are left with the Application Data

<hr>

### Disecting the Ethernet Frame

![[002 Disecting a Frame.png]]

- The diagram above shows encapsulation and decapsulation on both sides

1. Layers 5-7 have Application Data. The protocols used here are HTTPS (web data), IMAP (email data), and SSH terminal data
2. Layers 5-7 (Application Layers) gets encapsulated in Layer 4 (Transport Layer). The protocols used in Layer 4 are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol)
3. Layer 4 (Transport Layer) gets encapsulated in Layer 3 (Network Layer). The protocol found in Layer 3 is IP (Internet Protocol)
4. Layer 3 (Network Layer) gets encapsulated in Layer 2 (The Data Link Layer). The protocol in Layer 2 is MAC (Media Access Control)

 - Header information is also included, the header information tells the network how the data should be processed.

<hr>

### TCP Flags

- The header describes or Identifies the payload
- The Flags control the payload. The various TCP flags are below.
	- SYN -> Synchcronize sequence numbers
	- PSH -> Push the data to the application without buffering
	- RST -> Reset the connection
	- FIN -> Last packet from the sender

<hr>

### Maximum Transmission Unit (MTU)

- MTU describes the Maximum IP packet to transmit
	- But not fragment
- Fragmentation slows things down
	- Losing a fragment loses the entire packet
	- Requires overhead along the path#
- It is difficult to know the MTU all the way through the path
	- Automated methods are often inaccurate
	- Escpecially when ICMP (is filtered 