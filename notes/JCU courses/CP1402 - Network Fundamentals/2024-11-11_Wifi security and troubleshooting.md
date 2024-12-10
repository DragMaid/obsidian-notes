---
date: "2024-11-11"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Wifi security and troubleshooting
# Wifi security
+ Default: 802.11 standard -> no security
+ Authentication - allows access after password correct or with credentials
    -> MAC filtering - prevent AP from allowing devices not listed to access network
+ Encyption algorithms

# WPA (Wifi protected access)
+ Dynamically assigns every transmission its own key
+ 802.11i -> gives encryption key generation and management scheme TKIP (Temporal Key Integrity Protocol) 
=> Improve security for legacy WEP-based devices
+ TKIP with improvements:
    1. Message integrity
    2. Key distribution
    3. Encryption

# WPA2 (same, version 2)
+ uses stronger confidentiality methods
+ CCMP (Counter mode with Ciher Block Chaining) MAC (message authentication code) protocol
=> ensure data confidentiality (with encryption / packet authen by providing: )
    1. Message integrity - ensure packets from declared source
    2. Encryption - uses AES (advanced encryption standard) -> faster / more secure than TKIP


# Perosnal and Enterprise
+ The most secure communication is made possible by combining a
RADIUS server with WPA/WPA2
+ Known as WPA-Enterprise or WPA2-Enterprise
+ RADIUS (Remote Authentication Dial-in User Service) is an opensource authentication and authorisation service
+ A RADIUS server is used in cooperation with an authentication
mechanism called EAP
+ EAP (Extensible Authentication Protocol) provides the framework
for authenticating clients and servers
+ EAP functions alongside RADIUS by organising communications
with the network client devices, while RADIUS handles the actual
authentication on the server
![[Pasted image 20241111114106.png]]

# Other security configurations
Additional security options include the following:
+ AP and antenna placement
+ Geofencing
+ Guest network
+ Wireless client isolation
+ Captive portal
+ IoT access considerations

# Security threatst Wifi networks
+ war driving - hacker search for unprotected wireless networks (using laptop configured to capture wireless data transmissions)
+ war chalking - hacker draw symbols with chalk on sideewalk or wall near vulnerable AP -> make it known to other hackers
+ evil twin - rouge AP planted in networks's geological are -> pose as an authorised AP
+ WPA attack/cracking - interception of network keys communicated between stations and APs
+ WPS attack - cracking PIN to access APs settings (brute force)

# Wifi Network tools
Two types of software tools you should have:
+ Spectrum analyser – a device that can assess the quality of the wireless signal
+ Wireless analyser (Wi-Fi analyser) – software that can evaluate Wi-Fi network availability, optimise Wi-Fi signal settings, and help identify Wi-Fi security threats

List of capabilities common to wireless testing tools:
+ Identify transmitting access points, stations, and channels
+ Measure signal strength from an AP
+ Indicate the effects of attenuation, signal loss, and noise
+ Interpret signal strength information
+ Ensure proper association and reassociation between APs
+ Capture and interpret traffic
+ Measure throughput and assess data transmission errors
+ Analyse characteristics of each channel

# Pitfalls - Errors and where to troubleshoot
+ No connection - cannot connect to AP:
    1. Wrong SSID
    2. Encryption and protocol mismatch
    3. Incorrect passphrase
    4. Static channel utilization
    5. Mismatched RF band
    6. Mismatched standards
    7. Long AP association time

+ Slow connections – when dealing with slow Wi-Fi connections:
    1. Insufficient wireless coverage
    2. RF attenuation/signal loss
    3. Interference
    4. Channel overlap
    5. Wireless standard specifications
    6. Simultaneous wired and wireless connections
    7. Problems with firmware updates
    8. Incorrect antenna type
    9. Mismatched antenna polarisation
    10. Client saturation or overcapacity
    11. Client disassociation issues
