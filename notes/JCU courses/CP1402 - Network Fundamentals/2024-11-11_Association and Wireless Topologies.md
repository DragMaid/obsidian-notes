---
date: "2024-11-11"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Association and Wireless Topologies
# Association
+ Process where packets are exchanged between computer & access point -> gain internet access

# Scanning
+ Wireless devices survey surroundings for access point
    + Active scanning -> client takes initiative by sending special frame (or a probe)
    + Passivec scanning -> AP(access point) takes initiative -> listen or special signal (or beacon fame)

# SSID (service per identifier)
+ Unique character strin idenitfying AP
    + SSID is contained in beacon fame info
    + SSID configured in AP's config -> recommended to be changed from default

# Topologies
+ IEE terms -> reflect common topologies:
    + IBSS (independent basic service set) - use ad-hoc (used when needed) topology
        + Small number of modes -> installed closely -> direcly transmit (not interference with other devices)
    + BSS (Basic service set) 
        + Infrastructure topology - group of stations share a single access point
        + Identifer for nodes here is BSSID (basic service set identifer)
![[Pasted image 20241111111132.png]]
    + ESS (extended service set)
        + Use mesh topology - several access points are connected via same LAN network
        + APs configured - managed by a wireless LAN controller 
        + Clients here -> share special identifier called ESSID
        => Allow user to roam, change from AP to AP
		![[Pasted image 20241111111522.png]]:w

