# The Transport Layer
<hr>
- Transport Layer takes services from the session layer
- Then it passes the data down the stack to the Network Layer

<hr>
#### Responsibilities of the Transport Layer
- End to end message delivery
- Error checking

- The transport layer will also add a port number to tell the data which application it should go to
- Error checking -> Deals with making sure the packets being delivered are not duplicated or corrupted

<hr>
#### Transport Functions
- Message acknowledgement and traffic control
- Session multiplexing (takes several sessions and combines them into one logical link, while still keeping track of which message streams belong to which session)
- Service point addressing (The process of specifiying and defining the port value)

<hr>
#### Data Delivery
- UDP -> user Datagram Protocol
- TCP -> Transmission Control Protocol 

- These are the most common protocols used to deliver data

<hr>
#### Connectionless Transmission
- Receiver does not acknowledge receipt of the packet
- The sending device assumes the packet arrived successfully
- Enables faster commnunication between devices

<hr>
#### Connection Oriented Transmission
- Establish a connection before data is transmitted
- The 2 systems agree to various parameters such as the amount of bytes sent in each segment
- They agree to use Acknowledgement (ACK) and Synchronization (SYN) to guarantee that packets arrive successfully

<hr>
