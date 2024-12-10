---
date: 2024-10-13
location:
  - JCU courses/CP1402 - Network Fundamentals
hubs:
  - "[[networking|Networking]]"
urls:
---

# Transmission Control Protocol (TCP)
+ Part of the transport layer (layer 2)
+ Three characteristics of TCP:
    1. Object oriented: ensure a connection / session using [[three-way handshake]]
    2. Sequencing and [[checksum]]: send checksum - checked by destination device along with sequence number for each segmnet
    3. Flow control: control rate of transmission based on how quickly recipient can accept data


# TCP segment
![[Pasted image 20241013111139.png]]
+ Source port - Destination port
+ Sequence number - show where the real data is being stored in the stream of data segments
+ Acknowledgement number - value of what sender wants to receive -> shows that previous segment has been successfully transmitted
+ Header length - size of TCP header (depends)
+ Reservced - reserved bits for later use

+ URG (Urgent pointer field) - if set to 1 -> contain information for receiver
+ ACK (Acknowledgment field) - if set to 1 -> contain information for receiver
+ PSH - if set to 1 -> data sent to application without [[buffering]]
+ RST - if set to 1 -> request a connection reset
+ SYN - if set to 1 -> request synchronization of the sequence numbers between two nodes -> indicates no payload in this segment (only a small request) -> and ACK number be set to 1
+ FIN - if set to 1 -> this is last segment -> connection should be closed

+ Sliding-window size: show how many bytes sender can issue befor acknowledgment is received
-> perform flow cntrol -> prevnet receiver buffer from being overflowed with bytes
+ [[Checksum]]: allow receiving node to determine wether TCP segment became corrupted during transmission
+ Options: specify special options (e.g. max segment size, ...)
+ Padding: contains filter bits -> ensure size of TCP header multiple of 32 bits

![[Pasted image 20241013114842.png]]