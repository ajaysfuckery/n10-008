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
![[002 encapsulation and decapsulation.png]]
