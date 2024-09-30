---
date: "2024-09-25"
location: 
  - JCU courses/CP1402 - Network Fundametals/Week 3
hubs: 
    - "[[networking]]"
urls:
    - 
---

# network infrastructure

# Components of strucutred cabling
+ ANSI/TIA-568 Commercial Building Wiring Standard
-> optmize way to install cables, maximize performance, minimize upkeep (maintenance fee)
![[Pasted image 20240925141424.png]]

# From Demarc to a workstation
![[Pasted image 20240925141516.png]]
+ Entrence facility - Building A:
    + MDF (main distribution frame) - where all LANs ans WANs are connected (center)
    + Data room - enclosed space -> hold network equipments
    + Rack - hold the network equiments
    + [[2024-09-25_patch-pannel|pactch panel]]] - be mounted on wall or rack

+ One of DRs may contain [[2024-09-25_VoIP]] equipments

+ Data room - Building B:
    + IDF (intermidiate distribution frame) - similar to MDF but on a smaller scale (secondary hub)
    acts as a bridge that connect MDF to local workstations

+ Work Areas all three buildings:
    + Work area - just like the name
    + Wall jacks - ANSI/TIA standard calls for each wall jack to contain at least one voice (RJ-11) and one data outlet (Ethernet RJ-45)
![[Pasted image 20240925143437.png]]
![[Pasted image 20240925143457.png]]

+ Rack systems:
    + Types: 2-4-6 post / walled / ceiling-mounted / free-standing
    + Things to consider:
        + Height - Rack unit (RU or U) - standard 42U tall
        + Width - standard 19 inch frame
        + Depth - varies
    *** Multiple rows of racks -> split cold aisle / hot aisle for optimal cooling
![[Pasted image 20240925144045.png]]

# Cabling
## Types of cables
+ Patch cable - short / connectors both ends
+ Horizontal cabling - connects workstation to data room / switches
+ Backbone cabling - consists of calbes / wireless links -> connect entrace facility and MDF and IDFs

![[Pasted image 20240925144342.png]]
![[Pasted image 20240925144351.png]]

## Cable management
+ Termination - dont leave 1 inc exposed cable beforehand
+ Bend radius - dont exceed -> can affect data transmission
+ Continuity - cable tester verify
+ Loosely cinch cables
+ Cable coverings and conduits (pipe/channel) - avoid laying cables on floor (or have cord covers)
+ EMI sources - install 3 feets away from sources of EMI
+ Plenum cabling (area above ceiling tile or below subflooring) -> make sure sheath is plenum-rated
+ Grouding
+ Slack in cable runs 
+ Cables trays - use trays for easy maintenance
+ Patch panels - to organize
+ Company standards and inventory (varies)
+ Documentation
