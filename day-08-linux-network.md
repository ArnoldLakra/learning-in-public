# Linux Networking & Infrastructure Security Fundamentals 🌐🛡️

Day 4 focused heavily on network utilities, routing paths, packet analysis, and security auditing tools inside the Linux ecosystem.

## 🔍 1. Connectivity & Diagnostic Tools
* ping — Verifies network-level connectivity to a host using ICMP echo requests.
* traceroute vs tracepath — Maps the hop-by-hop network path packets take to a destination (tracepath doesn't require root privileges).
* mtr — (My Traceroute) Combines ping and traceroute into a live, real-time network diagnostic tool.
* watch — Runs a specified command repeatedly at intervals, allowing real-time monitoring of networking stats.

## 📊 2. Interface Configuration & Socket Statistics
* ip — The modern, versatile tool used to manage interfaces, IP addresses, and routing tables (replaces ifconfig).
* ifconfig — Legacy network interface configuration utility.
* iwconfig — Used to display and alter wireless network interface configurations.
* ifplugstatus — Detects the physical link state (cable plugged in or not) of local interfaces.
* ss — Modern utility to dump socket statistics, showing active TCP/UDP connections (replaces netstat).
* netstat — Legacy network statistics utility for monitoring ports and connections.

## 🛡️ 3. Security, Port Auditing & Routing
* nmap — A powerful network mapper used for security auditing, network discovery, and open port scanning.
* iptables — Interface to the Linux kernel netfilter framework, used to configure host-based firewalls and traffic routing.
* nc (Netcat) — The "Swiss Army knife" of networking; reads and writes data across network connections (useful for port scanning or reverse shells).
* telnet — Unencrypted protocol used to test manual TCP port banners and remote connections.
* route — Views and alters the IP routing table configuration.
* arp — Views or modifies the local Address Resolution Protocol (ARP) cache table.
## 🧠 4. Domain Name System (DNS) & API Tools
* nslookup — Queries internet name servers interactively to troubleshoot DNS issues.
* dig — (Domain Information Groper) The preferred modern tool for performing robust DNS lookups.
* whois — Queries public databases to locate ownership, registration, and block allocations of domains/IPs.
* curl vs wget — curl is designed to transfer data to/from a server via protocols (and outputs to stdout), whereas wget is optimized for downloading files/directories recursively.
* jq — A lightweight command-line JSON processor, highly powerful when paired with curl for filtering API data streams.
---
![alt text](<Screenshot 2026-06-30 154339.png>)
![alt text](<Screenshot 2026-06-30 154623.png>)
![alt text](<Screenshot 2026-06-30 154732.png>)