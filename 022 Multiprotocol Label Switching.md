# Multiprotocol Label Switching (MPLS)
<hr>
- Switching in this topic deals more with routing (Layer3 but also deals with Layer 2)
- Used to ensure reliable connections for applications in real-time
- It's a technique not a service
- It's expensive

- IP routing can be compared to tracking a package as if it passes through multiple destinations on the way to you

- MPLS routers establish highly efficient, pre-determined routes
- As a packet enters the network it gets assigned to a Forwarding Equivalence Class (FEC)
- Think of this as a Label, MPLS "stamps" the packet and this tells it to go a particular route
- All network routers that support MPLS have a specific table that specifies how specific FEC-type packets should be handled

- These routers allow MPLS to consistently handle the same type of packets
- Packets like those in VoIP (Voice over IP) or video conferencing can be mapped to suitable network routes with low latency
- Labels attatch information to the packet that is useful to routers

<hr>
#### MPLS features
- Not bound to any underlying technology
- Designed to improve performance 
- Commonly used between branch offices or enterprises requiring real-time applications

<hr>
#### MPLS Label Components
- Label -> Tells the packet which route to take
- Experimental -> Holds the bits used for quality of service, prioritizing the packets
- Bottom of the stack -> Informs the last router that it is the last router
- Time-To-Live -> How many hops a packet can make before it is discarded

<hr>
#### MPLS Pros and Cons
- Pros
	- Scalable service and provides good end-user-experience
	- Reduced network congestion
	- Improved bandwidth utilization
	- Secure mode of transport
	- Not as vulnerable to DoS attacks (Denial of Service)
- Cons
	- Doesn't provide encryption
	- More expensive than using public internet for sending traffic
	- Challenging to find a provider who can deliver coverage globally
	- Wasn't designed for cloud use
