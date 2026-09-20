Networking Fundamentals Lab

Notes and troubleshooting exercises from my networking study. I am building the networking foundation I need for IT support and SOC work.

---

Topics Covered

- TCP/IP and the OSI model
- IPv4 addressing and subnet masks
- Private and public IP addresses
- Default gateways
- DNS and DHCP
- ARP and NAT
- TCP and UDP
- LAN and WAN
- Routers, switches and firewalls
- Common ports and protocols

---

Commands I Use

- `ipconfig /all` — check Windows network configuration
- `ping` — test connectivity
- `tracert` — check the path to a destination
- `nslookup` — test DNS resolution
- `arp -a` — view the local ARP cache
- `ipconfig /release` and `ipconfig /renew` — renew a DHCP lease

---

Troubleshooting Practice

169.254.x.x address

I would check the network connection, adapter configuration and DHCP availability, then try renewing the lease.

Can ping 8.8.8.8 but not a hostname

This points me towards DNS. I would check the configured DNS server and test name resolution with `nslookup`.

Cannot reach a server

I would check the IP/hostname, DNS, gateway and connectivity first, then look at the required port, firewall, service availability and permissions.

---

Useful Ports

- 22 — SSH
- 53 — DNS
- 67/68 — DHCP
- 80 — HTTP
- 443 — HTTPS
- 445 — SMB
- 3389 — RDP

---

Related Lab Work

My Kali, Suricata, Splunk and Microsoft Sentinel labs use these networking fundamentals when reviewing IP addresses, ports, protocols, authentication traffic and security alerts.

Current focus: subnetting, DNS, DHCP, routing and network troubleshooting.

Progress still ongoing.
