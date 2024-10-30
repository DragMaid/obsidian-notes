---
date: "2024-10-13"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[Networking]]"
urls:
    - 
---

# three-way handshake
+ Consists of 3 parts: synchronize(SYN) - synchronize-acknowledge(SYN-ACK) - acknowledge(ACK)
1. SYN - sends synchronize sequece number (SYN) to destinated device - asking if a open connection is available
2. SYNC-ACK - sends back a synchronize-acknowledge (SYN-ACK) packet to first sender - packet consists of 2 numbers (device own SYN and ACK number, which is initiating device' SYN + 1)
3. ACK - send ACK number back to original sender -> after that connection is established -> transmission can begin
=> After that -> payload or data is sent
=> Sequence numbers will be increased by the number of bytes included in each received segment => confirm correct length of message received
![[Pasted image 20241013114633.png]]
