---
date: "2024-10-13"
location: 
    - JCU courses/CP1402 - Network Fundamentals
hubs: 
    - "[[networking|Networking]]"
urls:
    - 
---

# Encryption protocol
+ Encryption -> use cryptographic methods -> scramble data -> format that can only be read after reversing the cipher (method of encryption)
+ Purpose - to keep information private
+ Encryption methods are primarily evaluated by 3 benchmarks:
    1. Confidentiality (hiding / scrambling data so only destined reicipent has access)
    2. Integrity (oxford definition: quality of honest and strong morality - protecting data from unauthorized changes) 
    3. Availability (guaranteeing reliable access for authorized clients)
+ Priciples above form standard security model called CIA triad
![[Pasted image 20241013172735.png]]

# Key encryption
+ A key - random string of chars - woven into original data bits
    + generates a unique data block -> called ciphertext
    + key generated accordig to specific rules (algorithms)
+ Key encryption split into 2 categories:
    1. Private key encryption
    2. Public key encryption

# [[IPSec (Internet Protocol Security)]]
# [[SSL (Secure Sockets layer) & TLS (Transport Layer Security)]]
# Symmetric and Asymmetric encryption
+ Symmetric - use 1 key for both encryption and decryption
+ Asymmetric - use 2 keys instead
