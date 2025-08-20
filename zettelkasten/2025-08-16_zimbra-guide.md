---
date: "2025-08-16"
location: 
    - 
hubs: 
    - "[[Networking]]"
urls:
    - 
---

# zimbra-guide
## Vietnamese guide (partitioning) - this shit is quite like installing archlinux
+ Documnetation: Contabo [[VPS]]
+ Procedures in order to properly partition disk:
    ### **Setting up the partitions**
    1. list all disks parts "ls -la /dev/disk/by-uuid" - This contain all symlinks for disk parts by uuid value
    2. lsblk to list the partitions
    3. mkdir to create new directories
    4. mount disk to directory
    5. Write fstab to ensure that it the mounting stays after reboot
    ### **Setting up the dns**
    1. set the ip to point to the dns of mail.zimlab.com
    2. set the timezones for the machine
    3. change /etc/hosts to re-do first
    4. modifying the network
        + disable ipv6 on the machine (default on sysctl)
        + applying the config
        + Reduce the swapiness (controls how aggressively system move data from ram to swap space)
        + Updating grub (why do for both ?) (the sysctl only disable ipv6 at runtime while grub option disable every time the device is booted)
    ### **Package installation**
    ### **Setting up the ports and firewall**
        + -A ufw-before-input -m conntrack --ctstate INVALID -j ufw-logging-deny (append rule tobefore inpt chain - before incoming traffic - conntrack to check connecting tracking state - ctsate INVALI D to check for packages that don't belong to known / valid connection - -j to jump to logging deny chain - log as packet is denied)
        + -A ufw-before-input -m conntrack --ctstate INVALID -j DROP (only this -j DROP would actually drop the packet)
    ### **Setting up the dns service [[dnsmasq]]**
    + Install then configure
    + Change [[netplan]] back to 127.0.0.1 instead of fuckin localhost or something
    + Remove [[systemd-resolved]]
    + Do checking with dig command
    ### **Finally install zimbra**
    + Follow the guide
    + Setup ssh keys
    ### **Setup [[2025-08-16_Email_Authentication_Mehods#dkim|DKIM]] and [[2025-08-16_Email_Authentication_Mehods#dmarc|DMARC]]**
    ### **Setup policyd**
    ### **Setup ssl certificiate using Letsencrypt**
    ### **Setup fail2ban**
