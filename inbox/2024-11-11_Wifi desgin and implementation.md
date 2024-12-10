---
date: "2024-11-11"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Wifi desgin and implementation

# Determine the design
+ Home or small office network (SOHO network) -> might only need 1 AP
    + AP device combine switching, routing, other network functions 
    + connects wireless devices to LAN and acts as internet gateway
+ Include IoT (internet of things) devices
![[Pasted image 20241111112159.png]]

+ Consider where to install AP:
    1. distance
    2. type and num of obstacles
    3. coverage 
    4. interference
+ Larger WAN warrant more systematic approach to AP placement
+ site survey -> assesses client requirements, facilities characteristics, coverage areas
    -> determine AP arrangement -> ensure reliable connectivity

+ A thorough site survey may inlude:
    1. Study building blueprints -> identify obstacles
    2. consider Wifi AP -> wireless bridges -> create remote wired access
    3. consider if floors need more APs
    4. measure coverage and signal strength 
    5. test proposed locations
    6. test access from furthest
    7. consider obstacle material
    6. consider intergration with wired portions
![[Pasted image 20241111112707.png]]

# Configure Wifi connectivity devices
+ APs vary - standards support - atenna strength - others
+ Variables that need to be set:
    1. Admin password
    2. SSID and wether it should be broadcasted or not
    3. Security options
    4. DHCP is used or not
=> If something is wrong -> force reset all variables

# Configure wifi clients
+ Varies from one client to another
+ AP broadcasting SSID -> clients will detect -> offer user options
+ On-boarding - installing specific program / app on device -> give trusted access to certain portions of network
+ Off-boarding - removing programs that gave devices special permissions on network
    + Admin need a feature to allow them to off-board remotely (in case AP is lost or stolen) -> called remote wipe
