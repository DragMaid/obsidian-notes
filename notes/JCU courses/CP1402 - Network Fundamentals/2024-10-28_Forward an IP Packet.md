---
date: "2024-10-28"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Forward an IP Packet
+ when frame received at router interface
+ [[2024-09-26_2024-09-23_Media access control (MAC)|Media access control (MAC)]] addrs checked -> see wether frame is addressed to router interface or a [[broadcast]]
+ frame header & trailer are removed -> packet passed up to Layer 3 [[OSI Module]]
+ [[2024-10-28_Routing Table|routing Table]] examined -> check for a match with destination IP addr of packet
+ Match - identify IP addr of next hop interface
+ next hop IP - only used to look up [[2024-09-26_2024-09-23_Media access control (MAC)|Media access control (MAC)]] in [[2024-10-13_ARP-(Address-Resolution-Protocol|ARP (Address Resolution Protocol)]] table -> used to construct a frame
+ Packet placed into new frame (next hop MAC as destination addr)
+ Frame is queued on outgoing interface until transmitted
![[Pasted image 20241028162432.png]]