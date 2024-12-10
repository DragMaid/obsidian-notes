---
date: "2024-11-11"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[]]"
urls:
    - 
---

# Access Method
+ [[2024-11-11_WLAN Standards#80211-inovations]] MAC sercies -> append 48-bit physical addr to frame -> identify source & destination
+ Use same physical addressing scheme as Ethernet networks -> easy to combine with other IEEE networks
+ Wireless devices not designed to simultaneously transmit and receive

+ 802.11 standards specify use of [[2024-09-26_Carrier Sense Multiple Access (CSMA)]] procedures to access shared medium
    + use ACK packets -> verify transmission
    + Requires more overhead than 802.3

+ RTS/CTS (Request to send / Clear to send) -> ensures packets not inhibited by other transmission
=> Decrease network efficiency -> but become more efficient for large transmission packets

![[Pasted image 20241111101315.png]]
![[Pasted image 20241111101335.png]]