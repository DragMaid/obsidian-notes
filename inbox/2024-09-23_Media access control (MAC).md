---
date: "2024-09-23"
location: 
    - 
hubs: 
    - "[[networking]]"
urls:
    - 
---

# Media access control (MAC)

# MAC funtionality
+ Manage and determine the size of data being transmitted through Network Cable
+ Prevent clustering / collision of data being transmitted simultaneously
+ Interpretation: MAC (traffic controller) -> guide which lane of cars goes first (data transmission) -> so they don't crash (transmission collision)

# MAC methods of management
1. Carrier sense mutiple access with Collision Avoidance (CSMA / CA)
2. Carrier sense mutiple access with Collision Detection (CSMA / DA)
3. Demand Priority
4. Token Passing

# CSMA / CA
+ Configure each device to send a signal before any actions of data transmission
+ Other devices also programmed to keep watch for signals from other machines to cancel transmission if one is prepared to go
-> This method is ==slow== since devices experience delay from having to wait to receive signals from other devices

# CSMA / CD
+ Detect signal of payload right on cable line and notify client device for transmission turn
-> This method is indeed faster but not as efficient as (it can only detect huge payload)
-> transmission collision is more prompt to happen than method [[#CSMA / CA]]

# Demand priority
+ Utilize active hub to manage network of all its client
+ Devices have to be authorized to start any transmissions
+ Considered as a better version of [[#CSMA / CA]]

# Token passing
+ Data transmission is only allowed for devices wth an authorized token (the token last for a specific amount of time before being passed over to a lower priority device)
