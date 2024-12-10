---
date: 2024-10-13
location:
  - JCU courses/CP1402 - Network Fundamentals
hubs:
  - "[[networking|Networking]]"
urls:
---

# ARP (Address Resolution Protocol)
+ Works in conjunction with [[2024-10-04_IPv4]] -> discover MAC address of host or node on local network
+ Is a layer 2 protocol which uses [[Internet Protocol (IP)]] and relies on broadcasting - operates only within local network
+ ARP table - database of IP to MAC address mappings
+ ARP table contains two types of entries:
    1. Dynamic - created when client makes ARP request - could not be satisfied by data already in ARP table
    2. Static - those entered manually using ARP utility (arp command)
+ Command prompt: view Windows's workstation ARP table - use "arp -a"

![[Pasted image 20241013170643.png]]
![[Pasted image 20241028160931.png]]