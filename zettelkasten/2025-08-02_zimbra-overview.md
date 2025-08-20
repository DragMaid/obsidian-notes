---
date: "2025-08-02"
location: 
    - 
hubs: 
    - "[[]]"
urls:
    - 
---

# zimbra-overview
## Introduction
+ Zimbra Collab includes MTA, LDAP server, mailbox server - installed on one server - no additional manual configs

## Zimbra 10 Port Mapping
- 25 - smtp - mta - incoming to postfix
- 80 - http - mailbox / proxy / LDS - web mail client
- 110 - pop3 - mailbox / proxy - POP3
- 143 - imap - mailbox / proxy / LDS - IMAP
- 443 - https - mailbox / proxy / web mail client - HTTP over TLS
- 465 - smtps - mta - Incoming mail to postfix ocer TLS
