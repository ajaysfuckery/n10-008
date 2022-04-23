![[001 OSI model.png]]

#### What is the OSI model?
- Open Systems Interconnection Reference Model

#### It's a guide (thus the term model)
- Don't get wrapped up in the details

#### This is not the OSI protocol suite
- Most of the OSI protocols didn't catch on

#### There are unique protocols at every layer

#### A way to remember the layers of the OSI model is the following:
- All People Seem To Need Data Processing

- Application, Presentation, Session, Transport, Network, Data link, Physical


<hr>
### Layer 1 (The Physical Layer)
<hr>
- ##### The physics of the Network
	- Signaling, cabling, connectors
	- This Layer isn't about protocols

- ##### "You have a physical Layer problem"
	- Fix the cabling, punch-downs etc.
	- Run loopback tests, test/replace the cables, swap adapter cards


<hr>
### Layer 2 (The Data Link Layer)
<hr>
- ##### The basic network "language"
	- The foundation of communication is at the data link layer

- ##### The Data Link Layer uses Data Link Control (DLC) protocols 
	- Example: MAC (Media Access Control) address on ethernet

- ##### The Data Link Layer is sometimes known as "the switching layer"


<hr>
### Layer 3 (Network Layer)
<hr>
- ##### Also known as the routing layer

- ##### This is the layer that deals with IP addresses (Internet Protocol (IP))

- ##### Fragments frames to traverse different networks


<hr>
### Layer 4
<hr>
- ##### Sometimes known as the "post office layer"
	- This layer describes how data will be sent and where it will be sent to in a network

- ##### TCP (Transmission Control Protocol) & UDP (User Datagram Protocol) are used at this layer
	- This layer is used when you are accessing a webpage but the webpage is so large that it needs to be "split up" and put back together onto your device


<hr>
### Layer 5 (The Session Layer)
<hr>
- ##### The session layer is used for communication management between devices.
	- Start/Stop/Resume communication between 2 devices

- ##### Control Protocols and Tunneling protocols are used here, in order to begin the communication between one device and another


<hr>
### Layer 6 (The Presentation Layer)
<hr>
- ##### Just before we are able to view data we receive, the presentation layer must convert the data to a form that we can understand
	- Anything dealing with character encoding, application encryption will be done here

 - ##### This layer is often combined with the Application Layer


<hr>
### Layer 7 (The Application Layer)
<hr>
- ##### Layer 7 is the layer we get to see
	- If you are performing a file share using FTP or a name search with DNS or using a browser, you are using Layer 7 of the OSI model.


<hr>
### Real-world to OSI model
<hr>
Layer 1 -> *Cables, fiber and the signal itself*
Layer 2 -> *Switch forwarding or looking at MAC addresses*
Layer 3 -> *IP Addresses, Routers, Packets*
Layer 4 -> *UDP/TCP and port numbers dealing with both of these protocols*
Layer 5 -> *Control Protocols, Tunneling Protocols*
Layer 6 -> *Character Encoding, Application Encryption (SSL/TLS)*
Layer 7 -> *Your eyes*


<hr>
### How the Layers of the OSI model work
<hr>

**Application** ->        https://mail.google.com -> (Using a web-browser for example) 
**Presentation** ->      SSL encryption for sending information
**Session** ->               Link the presentation and the application together
**Transport** ->           TCP encapsulation
**Network** ->              IP encapsulation
**Data Link** ->             Ethernet
**Physical** ->               Electrical Signals