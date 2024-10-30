---
date: 2024-09-23
location:
  - JCU courses/CP1402 - Network Fundamentalss
hubs:
  - "[[networking]]"
urls:
---

# Definition of IP
+ IP adds its own network later header to segment (TCP) or datagram (UDP)
+ IP is the location (home address) that the internet network (shipper) uses to navigate and deliver your packages (data frames)
+ IP enables [[2024-10-13_Transmission Control Protocol (TCP)]] to internetwork - traverse more than 1 LAN segment / network type through a router
+ Unreliable, connectionless protocol - no guarantee the delivery of data and no session / connection is established before data transmission
=> Depends on TCP - ensure messages are put back together in right order - reaches correct application on receiving host
=> Personal interpretion: IP know the address, but TCP has the map to guide IP and shows it how to collect deliveries

# IP addresses
+ Static IP -> assigned manually by admin
+ Dynamic IP -> automatically assigned by [[DHCP]] server
+ Two types of IP addr -> IPv4 (32bits) and IPv6(128bits)

# [[2024-10-04_IPv4]]
# [[2024-10-06_IPv6]]
# [[2024-10-07_Internet-Control-Message-Protocal-(ICMP)|Internet Control Message Protocal (ICMP)]]

