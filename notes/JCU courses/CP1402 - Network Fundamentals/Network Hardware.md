# LANs and hardware
+ LAN or (Local area network) network contained locally -> requires connected devices to have compatible hardware
+  NIC or (network interface card) -> network port to connect device to a network (also known as network adapter)
+ A switch -> receives data from ports -> redirects to another port within its network
+ Physical topology used by this network is call star network
![[Pasted image 20240917175926.png]]
+ LAN can have several switches
+ A backbone -> central conduit -> connects segments of a network
+ A bus topology is when several devices are chained in a single line
+  A hybrid topology combines other topologies
![[Pasted image 20240917180215.png]]

# Routers
+ A router manages network between two or more networks -> network bridge
+ Routers can do the following:
    + Connect LANs and WANs to internet (SOHO or small office-home office network)
    + Interpret Layer 3 & 4 addressing
    + Calculate best path to get from A->B
    + Reroute traffic if first choice is broken & another path is availale

+ Some of the optional functions:
    + Filter broadcast transmission -> allow / prevent traffics 
    + Monitor traffic - report statistics
    + Diagnose problems - trigger alarms

+ Categories:
    + Core / Interior routers - direct data between networks in same [[autonomous system (AS)]]
    + Edge / Border routers - connect [[2024-10-28_autonomous system (AS)|autonomous system (AS)]] with outside network
    + Exterior routers - refers to any routers outside [[2024-10-28_autonomous system (AS)|autonomous system (AS)]]

+ Difference routers - switches:
	+ Router gateway between networks among many LANs
	+ A switch belongs to only one LAN 
![[Pasted image 20241028110648.png]]

# MANs and WANs
+ WAN (wide area network) -> group of LANs spread far away
+ MAN (metropolitan area network) -> group of connected LANs in the same geographical area
+ Both have different transmission methods and media than LANs
![[Pasted image 20240917180740.png]]

# Other network types
![[Pasted image 20240917180800.png]]
