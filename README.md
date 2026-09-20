Networking Fundamentals Lab

This repository documents my ongoing study and practical understanding of computer networking fundamentals.

The purpose is to build the networking knowledge required for IT support, cybersecurity and SOC analyst roles.

Progress still ongoing.

---

Networking Fundamentals

Topics covered:

- TCP/IP
- IPv4
- Public and private IP addresses
- Static and dynamic IP addresses
- Subnet masks
- Default gateways
- MAC addresses
- DNS
- DHCP
- ARP
- NAT
- LAN
- WAN
- VPN fundamentals
- Routers
- Switches
- Firewalls
- Network ports
- TCP and UDP

Progress still ongoing.

---

OSI Model

Layer 7 - Application
HTTP, HTTPS, DNS, SMTP

Layer 6 - Presentation
Encryption, encoding and data formatting

Layer 5 - Session
Establishing and maintaining communication sessions

Layer 4 - Transport
TCP and UDP

Layer 3 - Network
IP addresses and routing

Layer 2 - Data Link
MAC addresses and switches

Layer 1 - Physical
Cables, network adapters and physical connections

Progress still ongoing.

---

IP Addressing

Example:

192.168.1.25

An IPv4 address identifies a device on an IP network.

Private IPv4 ranges include:

10.0.0.0 - 10.255.255.255

172.16.0.0 - 172.31.255.255

192.168.0.0 - 192.168.255.255

Private addresses are normally used inside local networks.

Progress still ongoing.

---

Subnet Masks

Example:

IP Address:
192.168.1.25

Subnet Mask:
255.255.255.0

CIDR:
/24

The subnet mask helps determine which part of an IP address identifies the network and which part identifies the host.

Progress still ongoing.

---

Default Gateway

A default gateway allows a device to communicate with networks outside its local subnet.

Example:

Computer:
192.168.1.25

Gateway:
192.168.1.1

Traffic destined for another network can be sent to the gateway for routing.

Progress still ongoing.

---

DNS

DNS translates domain names into IP addresses.

Example:

google.com

↓

IP address

Useful command:

nslookup google.com

Basic troubleshooting scenario:

A computer can ping an external IP address but websites do not work by hostname.

Possible area to investigate:

DNS resolution.

Progress still ongoing.

---

DHCP

DHCP can automatically provide devices with network configuration including:

- IP address
- Subnet mask
- Default gateway
- DNS server

A Windows address beginning with:

169.254.x.x

can indicate that the device has assigned itself an APIPA address after failing to obtain an IPv4 address from DHCP.

Progress still ongoing.

---

TCP and UDP

TCP

Connection-oriented and designed for reliable delivery.

Examples include:

- HTTP/HTTPS
- SSH
- FTP

UDP

Connectionless with lower protocol overhead and no TCP-style delivery guarantee.

Common uses include:

- DNS queries
- Voice/video traffic
- Streaming and real-time applications

Progress still ongoing.

---

Common Ports

20/21 - FTP

22 - SSH

23 - Telnet

25 - SMTP

53 - DNS

67/68 - DHCP

80 - HTTP

110 - POP3

143 - IMAP

443 - HTTPS

445 - SMB

3389 - RDP

Progress still ongoing.

---

Networking Commands

ipconfig

View Windows network configuration.

ipconfig /all

View detailed adapter information.

ping

Test IP connectivity.

Example:

ping 8.8.8.8

tracert

View the network path towards a destination.

Example:

tracert google.com

nslookup

Test DNS resolution.

Example:

nslookup google.com

arp -a

View the local ARP cache.

Progress still ongoing.

---

Basic Troubleshooting Process

When a computer has no network access:

1. Check the physical or Wi-Fi connection.

2. Check the IP configuration.

ipconfig /all

3. Check whether the computer has a valid IP address.

4. Test the local TCP/IP stack.

ping 127.0.0.1

5. Test the default gateway.

ping <gateway>

6. Test an external IP address.

ping 8.8.8.8

7. Test DNS.

nslookup google.com

8. Use tracert when investigating the route towards a remote destination.

Progress still ongoing.

---

Troubleshooting Scenario 1

Problem:

Computer receives:

169.254.x.x

Possible cause:

The computer may have failed to obtain an IPv4 address from DHCP.

Checks:

- Network connection
- DHCP availability
- Adapter configuration
- DHCP lease renewal

Commands:

ipconfig /release

ipconfig /renew

Progress still ongoing.

---

Troubleshooting Scenario 2

Problem:

Computer can ping:

8.8.8.8

but cannot resolve:

google.com

Possible area:

DNS.

Checks:

nslookup google.com

Check configured DNS servers.

Progress still ongoing.

---

Troubleshooting Scenario 3

Problem:

A user can access some network resources but cannot connect to a particular server.

Checks could include:

- Server IP/hostname
- DNS resolution
- Ping/connectivity
- Correct network
- Required port
- Firewall rules
- Service availability
- User permissions

Progress still ongoing.

---

Cybersecurity Connection

Networking knowledge is important in cybersecurity because security analysts regularly investigate:

- Source IP addresses
- Destination IP addresses
- Network ports
- Protocols
- DNS activity
- Authentication traffic
- Firewall logs
- IDS alerts
- Network connections

My Microsoft Sentinel, Kali Linux, Suricata and Splunk labs build on these networking fundamentals.

Progress still ongoing.

---

Current Focus

I am continuing to develop my understanding of:

TCP/IP • IPv4 • Subnetting • DNS • DHCP • Ports • Routing • Network Troubleshooting • Network Security

Progress still ongoing.
