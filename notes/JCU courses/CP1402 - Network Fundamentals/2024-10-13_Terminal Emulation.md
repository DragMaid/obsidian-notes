---
date: "2024-10-13"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Terminal Emulation
+ Terminal emulator - allows user from one computer (client) - controls another device (host / server)
+ Example of commandline software - telnet and SSH
![[Pasted image 20241013173749.png]]

+ SSH (secure shell) - collection of protocols provides secure authentication - encryption
    + Protect you from:
        + Unauthoized access to host
        + [[IP spoofing]]
        + Interception of data in transit
        + [[DNS spoofing]]
    + Secure connection requires SSH running both ends
    + Allows password authentication - by public / private key generation

+ RDP (Remote Desktop Protocol) - used to connect and control remote computer (Microsoft)
+ VNC (Virtual Network Computing) - cross platform protocol [[RFB (remote frame buffer)]] - remotely control workstation or server
    + Run OSes on client computers
    + Remotely access computers / tablets / smartphones
    + Remotely control media equipment and surveillance systems
+ Out of band management - relies on dedicated connection between admin computer and other network devices
    + Remote management card - attached to network device console port
    + single device (console server / router) provides centralized management of all linked devices

# [[VPN (Virtual Private Networks)]]
