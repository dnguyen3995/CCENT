# *Internetworking*
## *Internetworking Basics*
* network segmentation - breaking large network into smaller network
* Things that can cause LAN traffic congestion:
	- too many host in a collision or broadcast domain
	- broadcast storm
	- too much multicast traffic
	- low bandwidth
	- adding hubs for connectivity to the network
	- a bunch of ARP broadcast
* Why breaking up a broach cast domain is so important?
	* when a host or a server sends a network broadcast every device on the network must read and process it.
	* router break up broadcast domain and collision domain
* 2 advantages for using router in your network
	* dont forward broadcast by default
	* filter network based on layer 3 network layer (IP address)
* 4 ways router function in your network
	* packet switching
	* packet filtering
	* internetwork communication
	* path selection
* Collision Domain - a device send out a packet on a network segment and every other device is forced to pay attention no matter what.
## *Internetworking Models*
* in late 1970s, the International Organization of Standard (ISO) created the Open Systems Interconnection (OSI) model to solve the problem of only computers from same manfufacture could talk to each other.
* the OSI model divide the communication system into logical groups call layer
* important befefits of using the OSI
	- divide network communiation process into smaller and simipler components, facillitating component development, design and troubleshooting
	- allows multi-vendor development through standardization of network components.
	- encourages industry standardization by clearly defining what functions occur at each layer of the model
	- allow various type of hardware and software to communicate
	- prevent changes in one layer from affecting other layers to expedite development.
## *OSI Reference Model*
	* Application 
		* provides a user interface
		* functions - file, print, message, database, and application services
		* where users communicates with the computer, and come into play only when access to the network will be needed.
		* Application layer is working as the interface between the application program and the next layer by providing a way for the application to send information down through the protocal call stack
	* Presentation 
		* presents data
		* Handles processing such as encryption
		* functions - data encryption, compression, and translation services
	* Session
		* Keeps different applications' data separate
		* functions - dialog control
	* Transport
		* provides reliable or unreliable delivery
		* performs error correction before retransmit
		* functions - end-to-end connection
	* Network
		* Provides logical addressing, which routers use for path determination
		* functions - routing
	* Data Link
		* combine packets into bytes and bytes into frames
		* provides access to media using MAC address
		* performs error detection not correction
		* functions - framing
	* Physical 
		* Moves bits between devices
		* Specifies voltage, wire speed, and pinout of cables
		* functions - physical topology