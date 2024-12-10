---
date: "2024-11-11"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# WLAN Standards
+ WLANs work at [[OSI Module]] layer 1 & 2
=> support TCP/IP higher-layer OSI protocols and operating systems
• Notable Wi-Fi standards
    • 802.11b, 802.11a, 802.11g, 802.11n, 802.11ac, and 802.11ax
    • 802.11n and later modify the way frames are used at the MAC
    sublayer (lower portion of the Data Link layer)
    • The LLC sublayer is primarily concerned with multiplexing, flow
    and error control, and reliability

# 802.11 inovations
1. Channel bonding
    + 2 adjacent 20-MHz -> bonded to make 40-MHz channel
    + More than double bandwidth available in a single 20-MHz channel
	![[Pasted image 20241111095554.png]]

2. MIMO (multiple input-multiple output)
    + Multiple access point and client device atennas -> issue signal to one or more receivers
    => Increases range and throughput

3. MU-MIMO (multiuser MIMO) 
    + Allows multiple atennas to service multiple clients simulatenously
    => Reduce congestion + faster data transmission
    => Available with WAVE 2 802.11ac products

4. OFDMA (Orthogonal Frequency Division Multiple Access)
    => More efficient multiuser functionality

5. Frame aggregation
    + combine many frames into one large frame
    + Techniques used to do this:
        + A-MSDU (Aggregated MAC service data unit)
        + A-MPDU (Aggregated MAC protocol data unit)
	![[Pasted image 20241111100441.png]]

# IEEE 802.11 Frames
+ specifies a MAC sublayer frame type
+ Frame types divided into 3 groups:
    + Management frames - association and reassociation
    + Control frames - medium access and data delivery (Ex: ACK or RTS/CTS frames)
    + Data frame - carry data between stations
![[Pasted image 20241111111839.png]]

# [[Access Method]]
# [[Association and Wireless Topologies]]
