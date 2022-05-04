# TCP Flags
<hr>
- Used to indicate the state of the connection, or to control traffic to a degree
- 3 most common flags:
	- SYN -> Synchronization
	- ACK -> Ackowledgement
	- FIN -> Finish

<hr>
#### SYN -> Synchronization
- Synchronization (also referred to as a 3 way handshake), is used in establishing the connection
- The initiating system says "I would like to initiate the transmission of data", the sender then says "ok begin"
- Only the first packet from the sender will have this flag set
- The other packets will not have this flag set because the receiver knows what to expect

<hr>
#### ACK -> Ackowledgement 
- Used to Acknowledge recipt of the packet
- Along with the Acknowledgement the sender also sends a SYN flag 

<hr>
#### FIN -> Finish
- Used to request termination of the connection for example, when the sender isn't sending information
- Last packet sent by the sender

<hr>
#### RST -> Reset 
- Also used to terminate the connection
- This is a forceful termination of connection, example -> when communication should not exist between the 2 hosts

<hr>
#### PSH -> Push
- Used when buffering needs to be managed
- Transport Layer might wait for the higher level layers to provide more data so that the packet is more full before sending the packet
- In some cases this is good, but in others it's bad. (Good => Fewer packets on the network, Bad => This is bad for real-time applications, such as video conferencing)

<hr>
#### URG -> Urgent
- Data is forwarded immediately
- Notifies Receiver to prioritize the packet over other packets
- Receivers are notified once all urgent packets are received

<hr>