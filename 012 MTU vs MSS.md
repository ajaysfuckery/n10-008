# MTU vs MSS
<hr>
Maximum Transmission Unit (MTU)
- Determines the largest packet size on a network

<hr>
#### Data Communications 
- MTU is specified at Layer 3 but it is constructed at Layer 2

<hr>
#### Increasing the MTU size
- Advantages
	- More data can be transmitted
	- Data transfer rates increase
	- Enables the use of Jumbo Frames

- Disadvantages
- Certain routers cannot handle jumbo frames

<hr>
#### MTU Optimal Size
- Ping command in windows and mac can be used to increase the size of the MTU
	- ping (URL/local sever or IP Address) -f -l xxxx
	- It is recommended to use 1500 bytes but it is also recommended to subtract some of the headers 
	- ping (URL/local server/IP) -d -s xxxx

<hr>
#### Adjusting MTU size
On windows use: netsh command 
On Linux use: ifconfig command 
On Mac: Change manually using system preferences 

<hr>
#### Maximum Segment Size (MSS)
- Largest amount of data a device can handle
- Data segment and header total size should be less than MTU size
