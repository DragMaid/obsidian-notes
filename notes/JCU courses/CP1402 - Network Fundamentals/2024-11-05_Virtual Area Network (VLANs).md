---
date: "2024-11-05"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Virtual Area Network (VLANs)
+ Groups ports on a switch -> forces some local traffic on switch to go through the router to be transmitted 
=> separate different workstation areas & limits traffic to a smaller broadcast domain

# Why use VLANs ?
+ Idetify groups of devices whose data be given **priority** handling
+ Isolate connections with heavy / unpredictable traffic patterns
+ Isolate devices that rely on legacy protocols -> incompatible with general traffic
+ Separate groups of users who need special secuirty or network functions
+ Configure temporary networks
+ Reduce cost of networking equipments

# How to setup VLANs?
+ Using a [[managed switch]] -> feature to confiure VLANs -> partition ports into groups
![[Pasted image 20241105112230.png]]

# VLANs on a single switch
+ First image -> frame transmitted directly from com A -> switch -> com B
+ Second image -> frame transmitted from com A -> router -> com B (com A, B now on different networks)
![[Pasted image 20241105112848.png]]

# VLANs can exist across many switches
+ VLAN 1 can directly send messages to each other via connected switches
+ VLAN 2 and 3 on the other hand have to communicate via the router
![[Pasted image 20241105113023.png]]
+ How does it manage this effectively ? Read [[2024-11-05_8021Q_tag|802.1Q]]]

# [[VLAN Trunks]]

# VLANs and subnets 
+ Most situations, each VLAN -> assigned own subnet of IP addrs
+ Sample network split into subnets (router sees 3 logical LANs connected to a single router port)
![[Pasted image 20241105114925.png]]
![[Pasted image 20241105115027.png]]

# [[Types of VLAN]]

# [[Dynamic VLAN assignment]]

# [[Troubleshoot and Secure VLANs]]
