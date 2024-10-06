---
date: "2024-10-06"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Resolving DNS query
![[Pasted image 20241006153605.png]]
+ local client -> local DNS resolver -> root DNS resolver -> TDL resolver for .edu -> resolver for mdc.edu
=> Just like asking for direction -> you ask from the big bois -> to the smaller people in the neighborhood -> till you get
to your final destination

+ Resolution process
    + Caching server != authoriative server ->  only resolve local clients
    + Nameservers within company -> may not have access to root servers
    + TLD name server might be aware of itermidiate nameserver (in between) rather than authoriative name server (ask many people
    for a person house address -> not just that person himself)

# Two types of DNS requests
+ Recursive lookup - spam message when you can't find the other person house address (demand an answer)
+ Iterative lookup - local servers issue queries to other servers (ask around wide area of neighborhood
=> does not demand an answer (only answer if they know))

# Resource Records in a DNS Database
+ Many types of records -> kept in DNS database: 
    + SOA (start of authority) record - gives information about zone (general)
    + A (address) record - store name-to-address mapping for host 
    + AAAA (address) record - store name-to-address mapping for host, IP address is IPv6
    + CNAME (canonical name) record - hold alternative names for host
    + PTR (pointer) record - for reversed lookups
    + NS (name server) record - indicates authoriative name server or a domain
    + MX (mail exhanger) record - identify mail server - used for mail traffic
    + SRV (server) record - identify host name / port of computer that host services
    + TXT (text) record - any kind of free form text

# DNS driver software
+ BIND (Berkeley Internet Name Domain) is the most popular DNS
server software
+ Open source - the term for software whose code is publicly
available for use and modification
+ Microsoft DNS Server is a built-in DNS service in the Windows
Server OS
+ Windows Server is capable of split-brain or split-horizon deployment,
which is used to handle internal clients and external clients
