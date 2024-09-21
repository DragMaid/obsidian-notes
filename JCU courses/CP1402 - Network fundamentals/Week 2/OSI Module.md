# OSI (Open Systems Interconnection)
+ 7 layered
+ categorize layers of communication
+ Separates to understand and simplify
![[Pasted image 20240918133636.png]]
# The seven-layer OSI model
![[Pasted image 20240918133753.png]]
## Physical layer :
+ transmit raw unstructured data bits -> receiving end point physical device (network hubs, cabling, repeaters, network adapters and modems) -> can be wired or wireless
## Data link layer:
+ Directly connect nodes -> perform node-to-node transfer -> package data into frames -> correct errors that occur at the physical layer(e.g switches)
+ Encompasses 2 sub-layers of its own:
	1. [[Media access control (MAC)]] -> flow control and [[Multiplexing]] -> acts like IP locally (distinction is that MAC verify device's physical address while IP for for device's network connection)
	2. [[Logical link control (LLC)]] -> flow / error control over physical medium and identifies line protocols
+ Protocols at these layers are programmed into firmware of [[NIC]] and other hardware
+ Type of network hardware-> determine DLL layer protocol used
![[Pasted image 20240918141952.png]]

## Network layer:
+ Receive frames from [[#Data link layer]]  -> deliver them to intended destinations (e.g routers)
+ Principle protocol used by this layer is [[Internet Protocol (IP)]]
+ Entire network layer message is called packet -> divide large packets -> smaller packets (fragmentation)
## Transport layer:
+ The transport layer manages the delivery and error checking of data packets. It regulates the size, sequencing, and ultimately the transfer of data between systems and hosts. One of the most common examples of the transport layer is [[Transmission Control Protocol (TCP)]] or [[User Datagram Protocol (UDP)]]
+ Protocols add control information at the beginning of payload (called header)
+ Encapsulation -> the process of adding a header to inherited layer above
+ Layer header addresses receiving end by using [[port number]]
![[Pasted image 20240918141246.png]]
## Session layer:
+ The session layer controls the conversations between different computers. A session or connection between machines is set up, managed. Session layer services also include authentication and reconnection. (e.g SSH connections -> expiration -> authentication)
+ Describes how data can be synced and recovered if messages don't arrive intact (packet loss)
## Presentation layer:
+ The presentation layer formats or translates data for the application layer based on the syntax or semantics that the application accepts. Because of this, it at times also called the syntax layer. This layer can also handle the encryption and decryption required by the application layer.
## Application layer:
+ Where users directly interact with received data packets -> The application layer identifies communication partners, resource availability, and synchronizes communication.
+ Utility services to the system -> (e.g. SNMP or Simple Network Management Protocol -> a program that monitor and gather information about network traffic)

** How to remember the layers easily **
![[Pasted image 20240918140131.png]]
## Overview of what data each layer represents
![[Pasted image 20240918142335.png]]

## Summary of how layers work together
![[Pasted image 20240918142357.png]]