---
date: "2024-11-05"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# VLAN Trunks
+ Each port on switch support [[2024-11-05_Virtual Area Network (VLANs)|Virtual Area Network (VLANs)]] is configured as one of 2 types of VLAN ports:
    1. Access port - connects switch to host
    2. Trunk port - connects the switch to a networking device (router, switch) -> manages traffic from multiple VLANs
![[Pasted image 20241105114215.png]]

+ A trunk is a single physical connection between switches through many logical VLANs
+ Trunking protocols assign and interpret [[2024-11-05_8021Q_tag|802.1Q Tag]]] or VLAN tags in Ethernet frames
+ Cisco's VTP (VLAN trunking protocol) - most popular
    + Allows changes to VLAN database on one switch - called stack master -> be communicated to all other switches on network
![[Pasted image 20241105114652.png]]
