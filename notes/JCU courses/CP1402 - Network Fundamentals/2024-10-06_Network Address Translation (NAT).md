---
date: "2024-10-06"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Network Address Translation (NAT)
+ A technique used to conserve public network address
+ A device acts as bridge (providing internal / private networks their own private IP) 
+ While internal devices when trying to connect to other external networks will use a mutual IP provided by NAT

# Two variations of NAT
+ SNAT (Source Network Address Translation) -> the gateway assign a default constant public IP address 
+ DNAT (Dynamic Network Address Translation) -> gateway has huge pool -> choose anything -> assign to local host

![[Pasted image 20241006111103.png]]
