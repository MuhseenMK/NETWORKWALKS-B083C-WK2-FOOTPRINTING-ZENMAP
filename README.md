# 🔍 Footprinting & Network Scanning

**Student:** Muhammad Muhsin Khamis  
**Program:** Cybersecurity  
**Platform:** NetworkWalks  
**Batch:** B083C  
**Week:** 02  
**Projects:** Footprinting with theHarvester (W2-PM4) & Network Scanning with Zenmap (W2-PM5)  
**Tutor:** Waqas Karim, CCIE

---

## 1. Project Overview

This project covered two key phases of a cybersecurity assessment:

1. **Footprinting & Reconnaissance** using **theHarvester** in Kali Linux.
2. **Network Scanning & Host Discovery** using **Zenmap** (the official Nmap GUI) on Windows.

The aim was to demonstrate how an ethical hacker moves from gathering publicly available information about a target domain to mapping live hosts on a local network.

All activities were performed within an authorised educational lab scope.

---

## 2. Objectives

- Use theHarvester to gather email addresses, subdomains, and hosts related to a target domain.
- Compare results from a single source (Baidu) vs. all available sources.
- Install and configure Zenmap on Windows.
- Identify the local IP address and LAN subnet.
- Use Zenmap's Ping Scan profile to discover live hosts.
- Identify IP and MAC addresses of the discovered hosts.
- Save the network topology as a PDF.

---

## 3. Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | OS used for theHarvester footprinting |
| theHarvester | Passive reconnaissance tool (emails, subdomains, hosts) |
| Windows 11 | OS used for Zenmap network scanning |
| Zenmap (Nmap GUI) | GUI for Nmap used for host discovery and topology mapping |
| Npcap | Packet capture driver bundled with Nmap for Windows |
| Windows CMD (`ipconfig`) | Local IP, subnet mask, and MAC address identification |

---

## 4. Activities Performed

### 4.1 Footprinting with theHarvester

#### Task 1 — Baidu, limit 1000

**Command:**
```bash
theHarvester -d microsoft.com -l 1000 -b baidu
