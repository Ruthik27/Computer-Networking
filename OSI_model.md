**Layers of OSI Model (Open Systems Interconnection):**
>Responsible for the actual physical connection between the devices.

>Physical Layer (Layer 1):
>>The physical layer contains information in the form of bits. It is responsible for transmitting individual bits from one node to the next. 
>>
>>Physical devices that interconnect each other
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
>>Responsible for the node to node delivery of the message. / for defining a comman way of interpreting these signals so network devices can communicate.
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
>>works for the transmission of data from one host to the other located in different networks./ allows different networks to communicate with each other through devices known as routers.
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
