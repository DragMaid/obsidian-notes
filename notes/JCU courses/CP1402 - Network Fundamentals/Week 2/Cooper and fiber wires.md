---
date: 2024-09-23
location:
  - JCU courses/CP1402 - Network Fundametals/Week 2
hubs:
  - "[[networking]]"
urls:
---

1. Coaxial cable
2. Twisted-pair cable
3. Fibre-optics

# Twisted-pair cable
+ Fast ethernets -> on pair send / get

# STP (shielded twisted pair)
![[Pasted image 20240923093744.png]]

# UTP (unshielded twisted pair)
+ No additional shielding

# Comparison [[#STP]] & [[#UTP]]
+ Throughput - same rates
+ Cost - they varry in cost (STP usually more expensive) 
+ Connector - same RJ-45 (register jack 45) 
+ Noise immunity - STP more resistant
+ Size and scalability - max segment length (both = 100 meter on Ethernets (data rate 1Mbps -> 10Gbps)

# Ethernet standard for TPC
+ Cable's category (cat 5e or cat 6) -> decide max network speed
+ NIC also rated for max net speeds
+ Most LANs support Fast Ethernet and Gigabit Ethernet
+ Fastest Ethernet standard (now) = 100GBASE-T
+ Two new standards:
    * 2.5GBASE-T
    * 5GBASE-T

![[Pasted image 20240923094558.png]]
+ Maximum distance is the same
+ Maximum transmission speed (Mbps) correlate to cable category name
+ All uses 2 pairs of twisted wires (the norm) 
(10 -> cat 3, 100 -> cat 5, 1000 -> cat 5/5e, 1000TX -> cat 6, 10G -> cat 6a/7)
# Cable pinouts
+ Two methods (provided by TIA/EIA or [Telecommunications Industry Association. Electronic Industries Alliance](https://csrc.nist.gov/glossary/term/telecommunications_industry_association_electronic_industries_alliance)) of inserting wires into RJ-45:
    + TIA/EIA 568A
    + TIA/EIA 568B

![[Pasted image 20240923095204.png]]

# Fibre-Optic Cable
+ Contains one or more glass or plastic fibres at its core
+ Data trabel by pulsing light from laser or LED 
+ Surrounded by a layer of glass or plastic called [[cladding]]: 
    - Less dense -> reflects light back to core in patterns
    - Reflections allow fibre to bend
+ Outside -> plastic buffer protects core:
    - Buffer is opaque, obsorbs escaping lights
    - Surrounded by Kevalar (polymetric fibre) strands
-> In conlusion: laser gun goes pew pew 

![[Pasted image 20240923095542.png]]

* Benefits:
    + Extremely high throughput
    + Very high noise resistance
    + Excellent security
    + Able to carry signals for longer distances

+ Drawbacks:
    + More expensive than twisted pair cable
    + Requires special equipment to splice

# SMF (Single Mode Fibre)
+ SMF consists of a narrow core 
    + Laser-generated light travels over one path, reflecting very little
    + The light does not disperse as the signal travels

+ SMF can carry signals many miles before repeating is required
+ SMF rarely used for shorter connections (due to high cost)
+ Internet backbone depends on SMF

![[Pasted image 20240923101017.png]]

# MMF (Multimode Fibre)
+ MMF contains a core (diameter > SMF core diameter)
+ Laser or LED -> light pulses -> travel different angles through MMF
+ Signals traveling over MMF experience greater attentuation than [[#SMF]]
+ Common usages:
    + Cables for routers / switches / servers on backbone of network
    + Cables to connect a desktop workstation to network
+ Transition SMF & MMF might occur at FDP (fibre distribution panel)

![[Pasted image 20240923101336.png]]

# Cable troublshooting tools

![[Pasted image 20240923101530.png]]

# Toner and Probe Kit
+ Tone generator (toner) -> device that issue a signal on wire pair
+ Tone locator (probe) -> device that emits a tone when electrical activity detected
+ Tone generators and tone locators are used to determine where wired pair terminates
![[Pasted image 20240923101758.png]]
+ Use tone locator on patch panel -> if the signal travel from patch panel all the way through ethernet cable installed within the wall -> if no problem then tone generator recieve signal -> generate sound 

# Multimeter
![[Pasted image 20240923101834.png]]

# Cable Continuity Tester
+ CCT -> test if a cable carries a signal to destination
+ Consists of 2 parts:
    + A base unit generates voltage
    + A remote unit detects voltage

+ Provide series of lights and some emit an audible tone (signal fail / pass)
+ Some verifiy UTP, STP wires are paired correctly
+ Fibre optic continuity testers -> issue light pulses on fibre -> see if pulse reach other end

# Cable Performace Tester
![[Pasted image 20240923102245.png]]

# OPM (Optical Power Meter)
![[Pasted image 20240923102327.png]]
