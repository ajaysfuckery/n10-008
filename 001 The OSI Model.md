# The OSI Model
<hr>
- The OSI model is just a model, you don't see it.
- The OSI model describes the functions of a networking system.
- The OSI model charactarizes computing functions for 2 computers to be able to communicate on a network.

<hr>
#### Purpose of the OSI model
- Guides vendors and developers
- Ensures products will interoperate

<hr>
#### OSI model benefits 
- Recognize how data is communicated over wide networks
- Understand how the OSI model helps new technologies adapt
- Outine how software and hardware work together
- Diagnose and troubleshoot issues
<hr>

#### Layered Approach
- Delivers more effective communications
- Ensures vendors focus on the entire protocol stack
- Divides data communication into seven different layers
<hr>

#### OSI Layers
7. Application Layer
6. Presentation Layer
5. Session Layer
4. Transport Layer
3. Network Layer
2. Data Link Layer
1. Physical Layer
<hr>

#### Relationships between Layers
| Host A | | Host B |
|---|---|---|
| Application | APDU | Application |
| Presentation | PPDU | Presentation |
| Session | SPDU | Session |
| Transport | Segment | Transport |
| Network | Packet | Network |
| Data Link | Frame | Data Link |
| Physical | Bits | Physical |
- The only Layer that matters on Host B is the same Layer as Host A (EX. The transport Layer on Host A interacts with the transport layer on Host B)

- Application Layer -> Application Protocol Data Unit
- Presentation Layer -> Presentation Protocol Data Unit
- Session Layer -> Session Protocol Data Unit
- Transport Layer -> Segment
- Network Layer -> Packet
- Data Link Layer -> Frame
- Physical Layer -> Bits

