
>Protocols
>>A protocol is the set of rules or algorithms which define the way how two entities can communicate across the network
>
>**Host name**
>>Each device in the network is associated with a unique device name known as Hostname.
>
>**Computer Networking**
>>An interconnection of multiple devices, also known as hosts, that are connected using multiple paths for the purpose of sending/receiving data or media. Computer networks can also include multiple devices/mediums which help in the communication between two different devices; these are known as **Network devices** and include things such as routers, switches, hubs, and bridges.
>
>**Network Topology**
>>The layout arrangement of the different devices in a network. Common examples include: Bus, Star, Mesh, Ring, and Daisy chain. 
>
>IP add.(Internet Protocol address / Logical Address)
>>the IP Address is the network address of the system across the network. To identify each device in the world-wide-web, the Internet Assigned Numbers Authority (IANA) assigns an IP.
>
>MAC Address (Media Access Control address / physical address)
>>The MAC Address is the unique identifier of each host and is associated with its NIC (Network Interface Card).
>
>Port
>>16-bit
>> 
>>A port can be referred to as a logical channel through which data can be sent/received to an application. Any host may have multiple applications running, and each of these applications is identified using the port number on which they are running. 
>>
>>Types:
>>
>>>Well known Ports	0 – 1023
>>>
>>>Registered Ports	1024 – 49151
>>>
>>>Ephemeral Ports	49152 – 65535
>
>Socket
>>The unique combination of IP address and Port number together are termed as Socket.
>
>DNS(Domain Name system)
>>DNS is basically a server which translates web addresses or URLs (ex: www.google.com) into their corresponding IP addresses. We don’t have to remember all the IP addresses of each and every website.
>
>ARP (Address Resolution Protocol)
>>Used to convert an IP address to its corresponding physical address(i.e., MAC Address).ARP is used by the Data Link Layer to identify the MAC address of the Receiver’s machine. 
>
>RARP(Reverse Address Resolution Protocol)
>>It provides the IP address of the device given a physical address as input. But RARP has become obsolete since the time DHCP has come into the picture.
>it provides the IP address of the device given a physical address as input. But RARP has become obsolete since the time DHCP has come into the picture.

Goals of Networks
>Networking Elements – The computer network includes the following networking elements:
>> <ol>
>> <li>At least two computers</li> 
>> <li>Transmission medium either wired or wireless</li>
>> <li>Protocols or rules that govern the communication</li> 
>> <li>Network software such as Network Operating System</li>
>> </ol>
>
>Network Criteria:
>> 1. Performance
>> 2. Reliability
>> 3.  Security
>
>Goals of Computer Networks
>>1. Resource Sharing
>>2. High Reliability
>>3. Inter-process Communication
>>4. Flexible access

Types of Network Topology
>Mesh Topology
>>In mesh topology, every device is connected to another device via particular channel.
>>
>>Ports that is required by each device is : N-1
>>
>>Total number of dedicated links required to connect them is : n to C to 2 i.e. N(N-1)/2
>>
>>ADVANTAGES:
>>>It is robust.
>>>
>>>Fault is diagnosed easily. Data is reliable
>>>
>>>Provides security and privacy.
>>
>>DISAVANT:
>>>Installation and configuration is difficult.
>>>
>>>Suitable for less number of devices
>>>
>>>Cost of maintenance is high.
>
>Star Topology
>>All the devices are connected to a single hub through a cable.This hub is the central node and all others nodes are connected to the central node.
>>
>> No of ports: 1 per device
>>
>>Dedicated links : 1 per device
>>
>>Passive : not intelligent hub such as broadcasting devices.
>>
>>Active : the hub can be intelligent. Active hubs have repeaters in them.
>>
>>ADAVNTAGE:
>>>Easy to set up.
>>
>>DISADVANT
>>>If the concentrator (hub) on which the whole topology relies fails, the whole system will crash down.
>>>
>>>Cost of installation is high.
>>>
>>>Performance is based on the single concentrator i.e. hub.
>
>Bus Topology
>>A network type in which every computer and network device is connected to single cable. It transmits the data from one end to another in single direction.
>>No bi-directional feature is in bus topology.
>>
>>ADVANTAGE
>>>Cables required to connect them is 1 i.e.- backbone cable and N drop lines are required
>>>
>>>Cost of the cable is less - it is used to built small networks
>>
>>DISADVANT
>>>If the common cable fails, then the whole system will crash down.
>>>
>>>If the network traffic is heavy, it increases collisions in the network.
>>>>To avoid - various protocols are used in MAC layer known as Pure Aloha, Slotted Aloha, CSMA/CD etc.
>
>Ring Topology
>>It forms a ring connecting devices with its exactly two neighboring devices.
>>> Number of repeaters are used for Ring topology with a large number of nodes -bcoz because if someone wants to send some data to the last node in the ring topology with 100 nodes, then the data will have to pass through 99 nodes to reach the 100th node. Hence to prevent data loss repeaters are used in the network.
>>
>>The transmission is unidirectional, but it can be made bidirectional by having 2 connections between each Network Node, it is called **Dual Ring Topology**
>>
>> Operations:
>>>1. One station is known as monitor station which takes all the responsibility to perform the operations.
>>>
>>>2. To transmit the data, station has to hold the token. After the transmission is done, the token is to be released for other stations to use.
>>>
>>>3. When no station is transmitting the data, then the token will circulate in the ring.
>>>
>>>4. There are two types of token release techniques :
>>>> **Early token** release releases the token just after the transmitting the data 
>>>>
>>>>**Delay token** release releases the token after the acknowledgement is received from the receiver
>>
>>ADVANTAGE
>>>The possibility of collision is minimum
>>>
>>>Cheap to install and expand.
>>
>>DISADVANT
>>>Troubleshooting is difficult in this topology.
>>>
>>>Addition of stations in between or removal of stations can disturb the whole topology.
>
>Tree Topology
>>This topology is the variation of Star topology. This topology have hierarchical flow of data.
>>
>>The various secondary hubs are connected to the central hub which contains the repeater. In this data flow from top to bottom or from bottom to top
>>
>>ADVANTAGE:
>>>It allows more devices to be attached to a single central hub
>>>
>>>It allows the network to get isolate and also prioritize from different computers.
>>
>>DISADVANT:
>>>If the central hub gets fails the entire system fails.
>>>
>>>The cost is high because of cabling.

Types of area networks:
>Local Area Network (LAN)
>>The group of computers and devices are connected together by a switch, or stack of switches, using a private addressing scheme as defined by the TCP/IP protocol. 
>>
>>Routers are found at the boundary of a LAN, connecting them to the larger WAN.
>>
>>Data transmits at a very fast rate as the number of computers linked are limited.Early LAN’s had data rates in the 4 to 16 Mbps range. Today, speeds are normally 100 or 1000 Mbps.
>>
>>The connections must be high speed and relatively inexpensive hardware
>>
>>LANs cover smaller geographical area (Size is limited to a few kilometers) and are privately owned. It covers a short distance, and so the error and noise are minimized.
>>
>>LAN is easy to design and maintain.
>>
>>A Communication medium used for LAN has twisted pair cables and coaxial cables
>>
>>The smallest LAN may only use two computers, while larger LANs can accommodate thousands of computers.
>>
>>A LAN typically relies mostly on wired connections for increased speed and security, but wireless connections can also be part of a LAN.
>>
>>The fault tolerance of a LAN is more and there is less congestion in this network.
>>
>Metropolitan Area Network (MAN)
>>covers a larger area than that of a LAN and smaller area as compared to WAN
>>
>>Connects two or more computers that are apart but resides in the same or different cities. It covers a large geographical area and may serve as an ISP (Internet Service Provider).
>>
>>Is designed for customers who need a high-speed connectivity.Speeds of MAN ranges in terms of Mbps.
>>
>>It’s hard to design and maintain a Metropolitan Area Network.
>>
>>It is costly and may or may not be owned by a single organization
>>
>>The data transfer rate and the propagation delay of MAN is moderate.
>>
>>Devices used for transmission of data through MAN are: Modem and Wire/Cable.
>>
>>The fault tolerance of a MAN is less and also there is more congestion in the network.
>>
>Wide Area Network (WAN)
>>Computer network that extends over a large geographical area, although it might be confined within the bounds of a state or country.
>>
>>A WAN could be a connection of LAN connecting to other LAN’s 
>>
>>The technology is high speed and relatively expensive.
>>
>>Types of WAN:
>>>Switched WAN
>>>
>>>Point-to-Point WAN
>>
>>Difficult to design and maintain.
>>
>>The fault tolerance of a WAN is less and there is more congestion in the network
>>
>>Communication medium -  PSTN or Satellite Link.
>>
>>Due to long distance transmission, the noise and error tend to be more in WAN.
>>
>>WAN’s data rate is slow about a 10th LAN’s speed, speed ranges from few Kbps to Mbps
>>
>>Propagation delay is one of the biggest problems faced here
>>
>>Devices used for transmission of data through WAN are: Optic wires, Microwaves and Satellites.
>
>PAN (Personal Area Network)
>
>SAN (Storage Area Network)
>
>EPN (Enterprise Private Network)
>
>VPN (Virtual Private Network)

**Layers of OSI Model (Open Systems Interconnection):**
>Responsible for the actual physical connection between the devices.

>Physical Layer (Layer 1):
>>The physical layer contains information in the form of bits. It is responsible for transmitting individual bits from one node to the next. 
>
>>Functions of the physical layer:
>>>1. Bit synchronization: The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at bit level.
>>>
>>>2. Bit rate control: The Physical layer also defines the transmission rate i.e. the number of bits sent per second.
>>>
>>>3. Physical topologies: Physical layer specifies the way in which the different, devices/nodes are arranged in a network i.e. bus, star or mesh topolgy.
>>>
>>>4. Transmission mode: Physical layer also defines the way in which the data flows between the two connected devices. The various transmission modes possible are: Simplex, half-duplex and full-duplex.
>
>>Hub, Repeater, Modem, Cables are Physical Layer devices

>Data Link Layer (Layer 2):
>>Responsible for the node to node delivery of the message.
>>
>>Main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer.
>>
>>When a packet arrives in a network, it is the responsibility of DLL to transmit it to the Host using its MAC address.
>>
>>The packet received from Network layer is further divided into frames depending on the frame size of NIC(Network Interface Card)
>>
>>DLL also encapsulates Sender and Receiver’s MAC address in the header.
>>
>>The Receiver’s MAC address is obtained by placing an ARP(Address Resolution Protocol- converting IP add to MAC add) request onto the wire asking “Who has that IP address?” and the destination host will reply with its MAC address.
>
>>Divided into two sub layers :
>>>Logical Link Control (LLC)
>>>
>>>Media Access Control (MAC)
>
>>Functions
>>>1. Framing: It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.
>>>
>>>2. Physical addressing: After creating frames, Data link layer adds physical addresses (MAC address) of sender and/or receiver in the header of each frame. 
>>>
>>>3. Error control: Data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.
>>>
>>>4. Flow Control: The data rate must be constant on both sides else the data may get corrupted thus , flow control coordinates that amount of data that can be sent before receiving acknowledgement.
>>>
>>>5. Access control: When a single communication channel is shared by multiple devices, MAC sub-layer of data link layer helps to determine which device has control over the channel at a given time.
>
>>Switch & Bridge are Data Link Layer devices.

>Network Layer (Layer 3) :
>>works for the transmission of data from one host to the other located in different networks.
>>
>>It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available.
>>
>>The sender & receiver’s IP address are placed in the header by the network layer.
>>
>>Segment in Network layer is referred as Packet.
>>
>>Functions:
>>>1. Routing: The network layer protocols determine which route is suitable from source to destination.
>>>
>>>2. Logical Addressing: In order to identify each device on internetwork uniquely, network layer defines an addressing scheme.The sender & receiver’s IP address are placed in the header by network layer. Such an address distinguishes each device uniquely and universally.
>
>>Network layer is implemented by networking devices such as routers.

>Transport Layer (Layer 4) :
>>Provides services to application layer and takes services from network layer.
>>
>>It is responsible for the End to End Delivery of the complete message. The transport layer also provides the acknowledgement of the successful data transmission and re-transmits the data if an error is found.
>>
>>• At sender’s side:
>>>Transport layer receives the formatted data from the upper layers.
>>>
>>>Performs Segmentation and also implements Flow & Error control to ensure proper data transmission.
>>>
>>>Also adds Source and Destination port number in its header and forwards the segmented data to the Network Layer.
>>>>The sender need to know the port number associated with the receiver’s application.
>>>>
>>>>Generally, this destination port number is configured, either by default or manually. For example, when a web application makes a request to a web server, it typically uses port number 80, because this is the default port assigned to web applications. Many applications have default port assigned.
>>• At receiver’s side:
>>>Transport Layer reads the port number from its header and forwards the Data which it has received to the respective application.
>>>
>>>It also performs sequencing and reassembling of the segmented data.
>
>>Functions:
>>>1. Segmentation and Reassembly: 
>>>>This layer accepts the message from the (session) layer , breaks the message into smaller units . 
>>>>
>>>>Each of the segment produced has a header associated with it. 
>>>>
>>>>The transport layer at the destination station reassembles the message.
>>
>>>Service Point Addressing: 
>>>>In order to deliver the message to correct process, transport layer header includes a type of address called service point address or port address. 
>>>>
>>>>Thus by specifying this address, transport layer makes sure that the message is delivered to the correct process.
>
>>Services:
>>1. Connection Oriented Service: It is a three-phase process which include
– Connection Establishment
– Data Transfer
– Termination / disconnection
The receiving device sends an acknowledgement, back to the source after a packet or group of packet is received. This type of transmission is reliable and secure.
>>2. Connection less service: It is a one-phase process and includes Data Transfer. In this type of transmission, the receiver does not acknowledge receipt of a packet. This approach allows for much faster communication between devices. Connection-oriented service is more reliable than
>
>>Transport Layer is called as Heart of OSI model.

>Session Layer (Layer 5) :
>>Responsible for establishment of connection, maintenance of sessions, authentication and also ensures security.
>
>>Functions: 
>>>1. Session establishment, maintenance and termination: The layer allows the two processes to establish, use and terminate a connection.
>>>
>>>2. Synchronization : This layer allows a process to add checkpoints which are considered as synchronization points into the data. These synchronization point help to identify the error so that the data is re-synchronized properly, and ends of the messages are not cut prematurely and data loss is avoided.
>>>
>>>3. Dialog Controller : The session layer allows two systems to start communication with each other in half-duplex or full-duplex.
>
>>All the below 3 layers(including Session Layer) are integrated as a single layer in the TCP/IP model as “Application Layer”.
>>
>>Implementation of these 3 layers is done by the network application itself. These are also known as Upper Layers or Software Layers.

>Presentation Layer (Layer 6) /  Translation layer:
>>The data from the application layer is extracted here and manipulated as per the required format to transmit over the network.
>
>>Functions:
>>>1. Translation : For example, ASCII to EBCDIC.
>>>
>>>2. Encryption/ Decryption : Data encryption translates the data into another form or code. The encrypted data is known as the cipher text and the decrypted data is known as plain text. A key value is used for encrypting as well as decrypting data.
>>>
>>>3. Compression: Reduces the number of bits that need to be transmitted on the network.

>Application Layer (Layer 7) / Desktop Layer:
>>At the very top of the OSI Reference Model stack of layers, we find Application layer which is implemented by the network applications.
>>
>>These applications produce the data, which has to be transferred over the network.
>>
>>This layer also serves as a window for the application services to access the network and for displaying the received information to the user.
>
>>Functions:
>>>1. Network Virtual Terminal
>>>
>>>2. FTAM-File transfer access and management
>>>
>>>3. Mail Services
>>>
>>>4. Directory Services
>
>>Ex: Application – Browsers, Skype Messenger etc.
























>TCP/IP model
>
>OSI model (Open Systems Interconnection)
>>It is a reference model that specifies standards for communications protocols and also the functionalities of each layer.
>
>DNS & DHCP
>
> 5 LAYER MODEL
>>PHYSICAL LAYER
>>> devices 
>>>
>>>bit - smallest representation of data(1 /0)
>>>
>>>modulation - varrying of charge 
>
>twisted pair cabel
>
>duplex communication - both direction data transfer
>>simplex C. - 
>>
>>full duplex C.
>>
>>half duplex C. - 
>
>network ports and patch panels
>
>>plug - RJ45 
>>>netw. ports - linked light , activity light 
>>patch panel
>>
>>DATA LINK LAYER - ETHERNET
>>>ethernet
>>>
>>>CSMA/CD - 
>>>
>>>MAC add. - 48 bit 2 to power 48 
>>>>OUI 
>>>>
>>>>hexa decimal 
>>>>
>>>>octact  - 8 bits
>
>>NETWORK LAYER (INTERNET LAYER) - IP 
>>
>>TRANSPORT LAYER - TCP/IP , UDP
>>
>>APPLICATION LAYER
>
>CABELS - point to point netw conn.
>
>>COPPER
>>>cat5, cat6, cat6e
>>>
>>>crosstalk
>>
>>FIBER (fiber optic cabels)
>>> uses pilses of light
>
>HUBS (ly2)
>>collision domain - one device at a time
>switch (ly 2)
>
>routers(ly 3) 
>
>>BGP 
>servers & clients
>
>uicast - 
>
>multicast -
>
>broadcast - 
>> address resolution protocol
>data packet (a to b)
>
>ethernet frame
>
>>preamble  - 8 bytes
>>
>>SFD 
>>
>> destination add. - 8 bytes
>>
>> source add.
>>
>>vlan - 4 bytes
>>
>>ether-type - 2 bytes
>>
>>payload - 0-1500 bytes
>>
>>frame check sequence - 4 bytes
>>
>>CRC


The Network Layer
>>IP(internet Protocol).
>>>IP add belongs to netw. not to the devices attactes to those networks.
>>>
>>>32 bit 
>>>
>>>8 bit - (0-255)
>>>
>>>Dynamic host Configuration Protocol - Dynamic Ip add
>>>
>>> Static IP add --
>>>
>>>IP datagram 
>>>> IPV4
>>>>>version 4 bits0
>>>>>
>>>>>header len - 4 bit (20 byte)
>>>>>
>>>>>service type - 8 bit
>>>>>
>>>>>total len - 16 bit
>>>>>
>>>>> identification - 16 bit
>>>>>
>>>>> flag - 
>>>>>
>>>>> fragmentation - 
>>>>>
>>>>> TTL - 8 bit
>>>>>
>>>>>protocol - 8 bit 
>>>>>
>>>>>header check - 16 bit
>>>>>
>>>>>source IP
>>>>>
>>>>>destination IP 
>>>>>
>>>>>options
>>>>> 
>>>>>padding
>
>>network and host id
>>>class A (1:3)
>>>> 0-126 (16 million)
>>>class B (2:2)
>>>>128-191 (64,000)
>>>class C (3:1)
>>>>192-224 (254)
>>>
>>>class D
>>>
>>>class E 
>>
>>CIDR -
>>>classless inter domain
>>>demarctation point
>>>CIDR notation
>>
>>ARP 
>>>ARP table
>>
>>subnetting
>>>subnet ID
>>>subnet mask (magic no)
>>
>>binary math
>>>OR
>>>
>>>AND
>>
>>routing 
>>>router
>>routing tables
>>
>>routing protocols
>>
>>>Interior Gateway Protocols
>>>>link state
>>>>
>>>>distance state
>>>Exterior Gateway Protocols
>>
>>IANA - 
>>ASN -
>>
>>non routable address space