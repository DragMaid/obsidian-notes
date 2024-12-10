---
date: "2024-11-05"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Troubleshoot and Secure VLANs
+ Common errors:
    + Incorrect VLAN assignment
    + Incorrect port mode (switch - endpoint -> access mode / switch to switch or routers -> trunk mode only if need to make VLANs)
    + VLAN isolation - can cut off group from rest of network

+ VLAN hopping - by attacker generates transmissions that appear to belong to a protected VLAN
=> acrosses VLANs to access data / inject virus
+ Two types of VLAN hopping:
    1. Double tagging - stack multiple VLAN tags in 1 frame (1 tag to get pass authentication, 1 tag leads to restricted addr) -> trick switch to forwarding to restricted VLAN
    2. Switch spoofing - make connection look like trunk connection -> switch may autoconfig port to trunk mode -> hacker can get VLAN data from that port 

+ Solutions:
    + Don't use default VLAN
    + Change native VLAN to unused VLAN
    + Disable auto trunking on switches that don't need to support traffic from multiple VLANs
    + Switches that only carry traffic for VLAns, configure all ports as access ports unless they are supposed to be trunk ports
    + Specify which VLANs supported per trunk instead of accepting range of VLANs
    + Use physical security method -> restrict access to network equipments
