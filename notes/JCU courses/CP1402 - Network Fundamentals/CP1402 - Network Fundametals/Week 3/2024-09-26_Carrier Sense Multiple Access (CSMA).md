---
date: "2024-09-26"
location: 
  - JCU courses/CP1402 - Network Fundametals/Week 3
hubs: 
    - "[[networking]]"
urls:
    - 
---

# Carrier Sense Multiple Access (CSMA)
# Definition of CSMA/CD
> A [[2024-09-26_2024-09-23_Media access control (MAC)|media access control (MAC)]] widely used in Ethernet / LANs
> Nowadays [[2024-09-26_Ethernet|Ethernet]] is [[Physical transmissions#full-duplex]] with star topology or point-to-point (direct connection)
> => No longer viable but still an included option

# How does CSMA/CD work
1. Check if sender is ready to transmit data packets
2. Check if transmission link is idle (no other device is currently occupying tunnel) -> sends
dummy data -> check for any collision signal -> decide activity of transmission link
3. Transmission & collision checking -> if during transmission -> collision detected
-> stop transmitting -> wait random time interval -> restart from step 1
4. If no problem -> completes frame transmission -> resets the counter

