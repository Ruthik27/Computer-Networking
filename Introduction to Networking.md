

>Protocols
>>A protocol is the set of rules or algorithms which define the way how two entities can communicate across the network

>**Host name**
>>Each device in the network is associated with a unique device name known as Hostname.

>**Computer Networking**
>>An interconnection of multiple devices, also known as hosts, that are connected using multiple paths for the purpose of sending/receiving data or media. Computer networks can also include multiple devices/mediums which help in the communication between two different devices; these are known as **Network devices** and include things such as routers, switches, hubs, and bridges.

>**Network Topology**
>>The layout arrangement of the different devices in a network. Common examples include: Bus, Star, Mesh, Ring, and Daisy chain. 

>IP add.(Internet Protocol address / Logical Address)
>>the IP Address is the network address of the system across the network. To identify each device in the world-wide-web, the Internet Assigned Numbers Authority (IANA) assigns an IP.

>MAC Address (Media Access Control address / physical address)
>>the MAC Address is the unique identifier of each host and is associated with its NIC (Network Interface Card).

>Port
>>16-bit 
>>A port can be referred to as a logical channel through which data can be sent/received to an application. Any host may have multiple applications running, and each of these applications is identified using the port number on which they are running. 
>>
>>Types:
>>>Well known Ports	0 – 1023
>>>
>>>Registered Ports	1024 – 49151
>>>
>>>Ephemeral Ports	49152 – 65535

>Socket
>>The unique combination of IP address and Port number together are termed as Socket.

>DNS(Domain Name system)
>>DNS is basically a server which translates web addresses or URLs (ex: www.google.com) into their corresponding IP addresses. We don’t have to remember all the IP addresses of each and every website.

>TCP/IP model
>
>OSI model (Open Systems Interconnection)
>>It is a reference model that specifies standards for communications protocols and also the functionalities of each layer.

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


>The Network Layer
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

>>>class D
>>>class E 

>>CIDR -
>>>classless inter domain
>>>demarctation point
>>>CIDR notation


>>ARP 
>>>ARP table

>>subnetting
>>>subnet ID
>>>subnet mask (magic no)

>>binary math
>>>OR
>>>AND

>>routing 
>>>router
>>routing tables

>>routing protocols

>>>Interior Gateway Protocols
>>>>link state
>>>>distance state
>>>Exterior Gateway Protocols

>>IANA - 
>>ASN -

>>non routable address space