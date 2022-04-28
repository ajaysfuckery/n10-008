# The Data Link Layer
<hr>
- Responsible for node-to-node data delivery
	- Receives data from the network layer and passes it on to the physical layer
- In the process it creates frames and adds physical addresses

<hr>
#### Responsibilites
- Physical addressing (MAC -> Media Access Cotnrol)
- Framing (Adding a frame onto the data)
- Access control (Determines which node has access to the data)
- Flow control (Determines how the data travels through the network)
- Error control (Helps increase the reliability of data transmission)

<hr>
#### Layer 2 - Transmission control
- Establishing and terminating links
- Media Access Management -> Determines which node has the ability to use the physical medium
- Flow control -> Helps prevent faster senders than slower receivers
- Error control -> Provides a mechanism to detect when frames are damaged or lost, so the data can be re-transmitted
- Access control -> specifies which node has control over the physical medium, when a single communication channel is being used by multiple nodes

<hr>
#### Layer 2 - Logical Link Control (LLC)
- Acts as an intermediary for the media access methods below and the Network Layer on the OSI model.
- Determines of the data will be *connectionless* or *connection oriented*

- ***Connectionless*** -> Imagine someone giving a speech. You can listen in or ignore it.
- ***Connection Oriented*** -> Imagine 2 people speaking. One is speaking to the other and vice versa

<hr>
#### Medium Access Control (MAC) aka Media Access Layer
- For connection to physical media
- MAC address:
	- 12 character hexadecimal value 
	- Unique to every network interface****