# The Application Layer
<hr>
- Serves as the interface for users and application processes to access network services 
	- In OSI model terms, the application layer is a collection of protocols that are required to support the application

<hr>
#### Layer 7 - Network Services
- The following services operate at layer 7 of the OSI model
	- FTP (File Transfer Protocol)
	- DHCP (Dynamic Host Configuration Protocol)
	- DNS (Domain Name Server)
	- SMTP (Simple Mail Transfer Protocol)
	- HTTP (Hyper Text Transfer Protocol)

- FTP -> Used to send files usually over the internet
- DHCP -> Used to assign IP addresses to devices
- DNS -> Used for name resolution
- SMTP -> Used for sending emails
- HTTP -> Used to by browsers

<hr>
#### Layer 7 - Functions
- Allows users to interact with applications
	- Application accepts user input and passes data down the network layers
	- Allows for easier application compatibilty and implementation
	- Applications do not have to be re-written for different types of network environments

```
	User                                      User    
	 v                                          ^
	Application Layer                       Application Layer
	 v                                          ^
	Data to presentation Layer       Data from presentation Layer
```

<hr>
#### Layer 7 - Application Examples
- Mail Services
- File Transfer, Access and Management

<hr>
#### Layer 7 - Browsers
- Provides internet access for all types of networking environments