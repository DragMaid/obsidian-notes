---
date: "2024-10-07"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Internet Control Message Protocal (ICMP)
+ Acts as communication between devices (client - server, peer-to-peer, ..)
+ A place to receive complaints that sent data did not get received or wether it was late
+ Only acts as intermediate -> no spot in [[OSI Module]]] -> does not manage data itself
=> Good for error reports, maintanence and troubleshooting 
=> Can also help agains [[Distributed Denial of Service (DDoS)]] attacks

# Features of ICMP
+ IMCP can indicate the following:
    + when part of a network is congested
    + when data fails to reach destination
    + when data has been discarded because TTL has expired
+ ICMP announces transmission failures to sender - no correction included
+ Provides critical information for troubleshooting
+ ICMPv6 on [[2024-10-06_IPv6]] networks performs functions of ICMP and ARP on [[2024-10-04_IPv4]] networks

