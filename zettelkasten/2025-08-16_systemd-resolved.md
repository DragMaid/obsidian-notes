---
date: "2025-08-16"
location: 
    - 
hubs: 
    - "[[Networking]]"
urls:
    - 
---

# systemd-resolved
+ A DNS resolver service built into systemd that handles DNS resolution for applcations, with primary purposes being:
    + Provide **stib resolution** (127.0.0.53 / loopback address)
    + Talk to DNS over TLS / DNSSEC / Split-DNS
    + Maintain per-interface DNS settings -> allow VPNs and specific interfaces can use different DNS servers
=> Beware as the service can cause conflict with [[2025-08-16_dnsmasq|dnsmasq]] if they are both listening on port 53

