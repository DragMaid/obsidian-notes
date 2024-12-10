---
date: "2024-11-05"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Types of VLAN
+ Default VLAN: preconfigured -> include all switch ports
+ Native VLAN: receives all untagged frames from untagged ports -> lead to security issues -> should be changed to unused 
+ Data VLAN: carries user-generated traffic (mail, web browse, database updates)
+ Management VLAN: used to provide administrative access to a switch
+ Voice VLAN: supports [[2024-09-25_VoIP]] traffic
+ Private VLAN: partition a VLAN broadcast domain into subdomains
    + Two types of secondary VLANs:
        1. isolated VLAN - completely isolate from hosts in same or other secondary VLANs
        2. community VLAN - hosts in same can directly communicate to each other - but not to other communicate VLANs

# Promiscuous port
=>  allow an external server / database to access the VLANs

![[Pasted image 20241105115723.png]]
