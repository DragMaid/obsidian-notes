---
date: "2024-09-25"
location: 
  - JCU courses/CP1402 - Network Fundamentalss
hubs: 
    - "[[networking]]"
urls:
    - 
---

# subnet mask
# Subnet mask definition
> As the internet protocol (IP) cannot manage and define subnet itself
> The router is required to use subnet mask method to categorize these subnetworks instead
> Example of a subnet 255.255.255.0
> Router will use this subnet mask to identify which device on its local network (same subnet) would receive the packet

# How subnet masks work
+ [[2024-10-04_IPv4|IPv4]] has 2 parts: network ID and host ID
+ subnet mask used -> determine which part IP is network ID and host ID
+ Number of 1s in subnet mask = number of bits of Network ID
![[Pasted image 20241028163733.png]]

# [[Calculating subnet masks]]
