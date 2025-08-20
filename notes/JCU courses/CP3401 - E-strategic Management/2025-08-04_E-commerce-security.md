---
date: "2025-08-04"
location: 
    - JCU courses/CP3401 - E-strategic Management
hubs: 
    - "[[]]"
urls:
    - 
---

# E-commerce-security
## What is good security ?
- Primary:
    + New techs 
    + Policies and procedures
    + Standards and laws
- Other factors: 
    + Time value of money
    + Cost vs loss
    + Security break at weakest link

## Customer and merchant perspective
+ Integrity: 
    + info received original or altered ?
    + data altered ?
+ Nonrepudiation:
    + no deny ?
    + can customers deny prods ?
+ Authencity: 
    + who tf is this ? how can I be sure?
    + who tf is this ? (user)
+ Confidentiality: 
    + Anoyone else can read ?
    + Anyone else not authorized can view ?
+ Privacy:
    + Can I control data about me ?
    + what use ? personal data from transaction ? info used in unauthorized manner ?
+ Availability:
    + can I access ?
    + is site operational ?

## Security threats
+ Client
+ Server
+ Communication pipeline
### Typical transaction
online store -> db server -> warehouse -> customer bank -> merchant bank -> ISP -> customer -> shipping

## Security Environment

## Common Security Threats
+ Credit card fraud / theft
+ Identity fraud / theft
+ Spoofing - disguising communication from unknown source
+ Pharming - directing internet users to bogus web -> mimic appearance of real one
+ Spam (junk) - websites
    - Link farm: irrelevant msg over internet -> many users -> advertise / spread malware
+ Sniffing - monitor / capture data packets through network
+ Denial of service (DDOS)
+ Insider attack (spy employee)
+ Poorly designed software
+ Social network security issues
+ Cloud security issues

## Technology solutions
+ Protect communication - encryption
+ Secure channels for commute - SSL, TLS, VPNs, Wifi
+ Protect network - firewalls, proxy servers, IDs, IPs
+ Protect server / client - OS security, anti-virus software

## Simple cryptography
+ original msg -> recipient public key -> msg encrypted cipher text -> internet -> recipient private key -> decrypt -> original msg

## SSL / TLS
+ request secure session - grant secure session
+ exchange certificates

## Payment system
+ credit / debit cards

### How online card transaction work
1. computer purchase
2. ssl / tls provide secure connection 
3. merchant software contact cleaning house
4. cleaning house verify issuing bank account 
5. issuing bank credits merchant bank account 
6. monthly statement issued with debt for purchase
