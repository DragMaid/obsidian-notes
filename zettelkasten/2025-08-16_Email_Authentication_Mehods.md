---
date: "2025-08-16"
location: 
    - 
hubs: 
    - "[[]]"
urls:
    - 
---

# Email Authentication Methods
+ Help prevent spammers / phishers / unauthroized parties from sending emals on behalf of a domain that they do not own
+ [[#DKIM]] and [[#SPF]] kind of like a busines licenese or doctoral degree that proves you are legit
+ [[#DMARC]] on the oter hand tells the mail servers what to do when the 2 above fail (like marking the mail as spam / dropping / sending it to another department for proper validation)
+ All of the 3 above are sstored within the [[2024-10-06_Domain-Name-System-(DNS)|Domain Name System (DNS)]]

## DKIM
+ Full name: DomainKeys Identified Mail
+ How: it allow owner to sign their emails from their domain. Uses public key cryptography to encrypt / verify the signature. DKIM record store domain's public key / private key is kept by sender and signs the header of the email with this key / receiver now use public key to verify the private key

## SPF
+ Full name: Sender Policy Framework
+ How: a way for a domain to list all servers they send emails from (to confirm if the sender is trustworthy or not). The SPF records list all the ip addresses of all the servers that are allowed to proceed to inbox

## PTR
+ Full name: DNS Pointer Record
+ How: it provides the the domain name associated with an IP address (Opposite of the A record - which provide the IP address associated with domain name)
=> Used for reverse DNS lookups (get domain names from the ips - reversed of dns lookup)

## A record (Address record)
+ example.com   IN   A   93.184.216.34
+ Maps domain name to ipv4 address

## MX record (Mail exchange record)
+ example.com   IN   MX   10   mail1.example.com
+ example.com   IN   MX   20   mail2.example.com
+ Directs email for a domain -> mail server that handles it
+ (10 / 20 means the priority of that server - lower number = higher priority)

## DMARC
+ Full name: Domain-based Message Authentication Reporting and Conformance 
+ How: Saves a record of rules and instructions of what to do after the 2 above tests failed - they can be quite flexible - whether to quaratine / flag or send logging reports to another admin is viable
