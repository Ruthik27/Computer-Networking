**Design issues**

>The data link layer in the OSI (Open System Interconnections) Model, is in between the physical layer and the network layer. This layer converts the raw transmission facility provided by the physical layer to a reliable and error-free link.

* Services to the Network Layer
>In the OSI Model, each layer uses the services of the layer below it and provides services to the layer above it. The data link layer uses the services offered by the physical layer.The primary function of this layer is to provide a well defined service interface to network layer above it.
>*Types of services:*
>>Unacknowledged connectionless service.
>>Acknowledged connectionless service.
>>Acknowledged connection - oriented service.

* Framing
>The data link layer encapsulates each data packet from the network layer into frames that are then transmitted.
>*Frame has three parts:*
>Frame Header
>>Payload field that contains the data packet from network layer
>>Trailer

* Error Control
>The data link layer ensures error free link for data transmission.
>*Issues faced:*
>>Dealing with transmission errors
>>Sending acknowledgement frames in reliable connections
>>Retransmitting lost frames
>>Identifying duplicate frames and deleting them
>>Controlling access to shared channels in case of broadcasting

* Flow Control
>The data link layer regulates flow control so that a fast sender does not drown a slow receiver. When the sender sends frames at very high speeds, a slow receiver may not be able to handle it.
>There will be frame losses even if the transmission is error-free.
>*Common approches:*
>>Feedback based flow control.
>>Rate based flow control.
---
**Flow Control Protocols:**
* Unrestricted Simplex Protocol / UTOPIA
>Simplest though unrealistic protocol.
>
>Data is transmitted in one direction only. Both the transmitting and receiving Network Layer are always ready and the proceeding time can be ignored. An infinite buffer space is available and also communication between a Data Link Layer never damages or looses frames.
>
>The protocol consists of two distinct procedures, a sender and a receiver. The sender is in the Data Link Layer of the source machine and the receiver is in the Data Link Layer of the destination machine. No sequence numbers and acknowledgments are used, only event type of possible frame_arrival i.e. an arrival of an undamaged frame is bothered.

>The sender is in an infinite while loop just sending data out on to the line as fast as it can. The body of the loop consist of three actions, 
>>go fetch a packet from the Network Layer, 
>>construct the outbound frame and 
>>send the frame on its way. 
>
>Only the information field of the frame is used by this protocol, because the other fields have to do with error and flow control and these are no errors or flow control restrictions here.

* Stop and Wait
>The sender sends one frame and wait for acknowledgment from receiver side.Once the receiver receives the frame, it sends an acknowledgment frame back to the sender.
>
>Efficiency of Stop-and-Wait Protocol is worse.
>>Sender window size of Stop-and-Wait Protocol is 1.
>>Receiver window size of Stop-and-Wait Protocol is 1.
>
>In Stop-and-Wait Protocol, sorting is not necessary.
>
>Stop-and-Wait Protocol is half duplex.
>
>Efficiency of Stop-and-Wait Protocol is : 1/(1+2*a)
* Sliding Window
>The sender sends more than one frame to the receiver side and re-transmits the frame(s) which is/are damaged or suspected.
>
>Efficiency of sliding window protocol is better.
>>Sender window size of sliding window protocol is N.
>>Receiver window size of sliding window protocol may be 1 or N.
>
>In sliding window protocol, sorting may be or may not be necessary.
>
>Sliding window protocol is full duplex.
>
>Efficiency of sliding window protocol is : N/(1+2*a)
---
* Hamming Code
>Hamming code is a set of error-correction codes that can be used to detect and correct the errors that can occur when the data is moved or stored from the sender to the receiver. It is technique developed by R.W. Hamming for error correction.

*Hamming Code | Error detection - https://youtu.be/1A_NcXxdoCc*

*Error Correction with Example | Hamming code | CN | Computer Networks | https://youtu.be/nUwGf5ZgqsA*

* Redundant bits –
>Redundant bits are extra binary bits that are generated and added to the information-carrying bits of data transfer to ensure that no bits were lost during the data transfer.
The number of redundant bits can be calculated using the following formula:
>>2^r ≥ m + r + 1 
>>where, r = redundant bit, m = data bit


* Parity bits –
>A parity bit is a bit appended to a data of binary bits to ensure that the total number of 1’s in the data is even or odd. Parity bits are used for error detection. There are two types of parity bits:
>>Even parity bit:
>>>In the case of even parity, for a given set of bits, the number of 1’s are counted. If that count is odd, the parity bit value is set to 1, making the total count of occurrences of 1’s an even number. If the total number of 1’s in a given set of bits is already even, the parity bit’s value is 0.
>>
>>Odd Parity bit:
>>>In the case of odd parity, for a given set of bits, the number of 1’s are counted. If that count is even, the parity bit value is set to 1, making the total count of occurrences of 1’s an odd number. If the total number of 1’s in a given set of bits is already odd, the parity bit’s value is 0.
---
**WAN Technologies**
*Layer2 Protocols* for point to point serial links.
>Data from lan pasiing through wan is converted first (called as encapsulation) this data can be converted under 2 protocols - HDLC & PPP 

>*Wan encapsulation protocols:*
>* High-level Data Link Control (HDLC)
>>HDLC is a Layer 2 protocol (see OSI Model for more information on Layers). HDLC is a simple protocol used to connect point to point serial devices. For example, you have point to point leased line connecting two locations, in two different cities. HDLC would be the protocol with the least amount of configuration required to connect these two locations. HDLC would be running over the WAN, between the two locations. Each router would be de-encapsulating HDLC and turning dropping it off on the LAN.
>>2 Versions:
>>>Standard Version.
>>>Cisco Proprietary.
>>No support authentication, Compression & error correction


>* Point to Point Protocol (PPP)
>>PPP originally emerged as an encapsulation method for transporting IP traffic over point-to-point links. It provides router-to-router and host-to-network connections over both synchronous and asynchronous circuits, for example, a leased line in case of synchronous and dial-up connections for asynchronous circuits. It is an enhancement over HDLC because it first of all provides link configuration, quality testing and error detection, but also additional capabilities like authentication, multilink bundles, and constant link monitoring.
>>
>>Standard Protocol
>>Supports authenticaton, compression & error correction
>>>• PAP (Password Authentication Protocol)
>>>>simplest Authentication method. It uses 2-way handshake. Both end send the passwords in “clear text” in this method. And passwords are exchanged only at the beginning.
>>
>>>• CHAP (Challenge Handshake Authentication Protocol)
>>>>more complex Authenticaion method. CHAP uses 3-way handshake and with this mechanims it checks the remote node periodically. CHAP uses MD5 hash. One end sends “Hash” to other node and the other node also sends a hash. If the hashes are same, then the communication starts.
>>
>>>NCP (Network Control Program)
>>>LCP (Link Control Protocol)
