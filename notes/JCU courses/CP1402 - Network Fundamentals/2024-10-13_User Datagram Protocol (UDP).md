---
date: 2024-10-13
location:
  - JCU courses/CP1402 - Network Fundamentals
hubs:
  - "[[networking]]"
urls:
  - https://www.rfc-editor.org/rfc/rfc768.html
---

# User Datagram Protocol (UDP)
+ Unreliable, connectionless protocol
    + No [[2024-10-13_three-way handshake]] is performed
    + Does not guarantee delivery of data
+ UDP provides no error checking, sequencing, flow control -> much faster / more efficient than TCP
+ Usage:
    + Good for live audio / video transmissions
    + More efficient carring messages that fit within 1 data packet
+ UDP header - 4 fields:
    1. Source port
    2. Destination port
    3. Length
    4. Checksum - optional for [[2024-10-04_IPv4]] - compulsory for [[2024-10-06_IPv6]]

