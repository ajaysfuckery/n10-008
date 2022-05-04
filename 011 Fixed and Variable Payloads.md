# Fixed/Variable Payloads
<hr>
#### Payload
- The actual data being transmitted

<hr>
#### Payload Examples
```
Computer One -> Sending System              Computer Two - Receiving System
		Packet                                         ^
		   V                                           ^
Header Payload Field Flag <--- Data Link Layer---> Header Payload Field Flag
	       V___________________________________________^	   
```

- The data link layer is the last layer where data transmission occurs before it is put across the wire

<hr>
#### Fixed Payload
- Frames become a fixed size
- When you have a fixed payload size, it can be more efficient

<hr>
#### Variable Payload
- A pattern is used to determine the frame size
- One frame might be larger than the other

<hr>
