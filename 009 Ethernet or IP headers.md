# Ethernet/IP Headers
<hr>
#### OSI Layers
The following layers of the OSI model are used in data communication
- Ethernet -> Layer 2
- IP Header -> Layer 3
- TCP/UDP Header -> Layer 4

<hr>
#### Ethernet Frame Format
| Preamble | SFD | Destination Address | Source Address | Length | Data | CRC |
|---|---|---|---|---|---|---|
	| 7 Bytes | 1 Byte | 6 Bytes | 6 Bytes | 2 Bytes | 46-1500 Bytes | 4 Bytes

1. Preamble -> Pattern to indicate the start of the frame & to allow the recipient to establish synchronization
2. Startup Frame Delimiter -> Indicates that the frame is starting 
3. Destination Address -> Mac Address to which the data is being sent to
4. Source Address -> MAC Address to which the data is being sent from
5. Length -> Indicates the entire length of the frame
6. Data -> The Actual data the user wants to send 
7. Cyclical Redundancy Check -> Mathematical code generated from Destination Address, Source Address and Length and Data. 

<hr>
#### Extended Ethernet Frame (Ethernet II Frame)
| DA | SA | Type | DSAP | SSAP | Ctrl | Data | FCS |
|---|---|---|---|---|---|---|---|
| 6 Bytes | 6 Bytes | 2 Byte | 1 Byte | 1 Byte | 1 Byte | 46 Bytes | 4 Bytes |

*(From Left to Right)*
1. Destination Address -> MAC Address to which the data is being sent to
2. Source Address -> MAC Address in which the data is being sent from
3. Type -> Designates Ethernet as the type
4. Destination Service Access Point -> Specifies the Logical Address of the Receiving Machine 
5. Source Service Access Point -> Specifies the Logical Address of the Sending machine 
6.  Control -> Specifies if the connection is Connectionless or Connection-Oriented 
7. Data -> The Data that you want to send across the network
8. Frame CheckSum -> Handles Error checking 
<hr>
#### IPv4 Header
- IP Header -> 20 bytes in length, Designates the Source and Destination Addresses using Logical Addressing (IP) not the MAC address
- Also includes information as to which version of IP is being used, the length and the checksum & TTL (Time To Live)
- TTL gives the data a lifespan, this means that after a certain time, the data should be deemed as unreliable and should be re-transmitted

<hr>
#### TCP Header 
- Ranges from 20-60 bytes in size and is used to specify the TCP port being used
- Since TCP communciations are Connection-Oriented, TCP uses Ackowledgements to guarantee packet delivery
- Monitors the state of the connections

<hr>
#### UDP Headers
- Specifies the port being used for the connection 
- A checksum value is used to validate the structure of the data only
- Fragmentation occurs in the TCP and UDP headers

<hr>
