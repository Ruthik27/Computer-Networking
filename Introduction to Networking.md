
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