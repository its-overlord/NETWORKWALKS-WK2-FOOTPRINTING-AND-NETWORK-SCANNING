# NETWORKWALKS-WK2-FOOTPRINTING-AND-NETWORK-SCANNING

**Week 2 Project | NetworkWalks Cybersecurity Internship 2026**

![Cybersecurity](https://img.shields.io/badge/Domain-Cybersecurity-blue)
![Internship](https://img.shields.io/badge/Program-NetworkWalks-red)
![Week](https://img.shields.io/badge/Week-02-green)

## 📌 Project Information

| Category | Details |
|---|---|
| Internship | NetworkWalks Cybersecurity Internship 2026 |
| Project | W2-PM-FINAL – Penetration Testing Report |
| Selected Module | W2-PM1 – Multiple Kali Tools |
| Compulsory Module | W2-PM5 – Zenmap Scanning |
| Domain | Cybersecurity & Ethical Hacking |
| Author | Uche Chimezie |
| Date | 19 November 2026 |

---

## 📖 Project Overview

This project involved two practical cybersecurity activities: **Footprinting & Reconnaissance** and **Network Scanning**.

The first activity involved using multiple Kali Linux tools to conduct reconnaissance against the `networkwalks.com` domain. The objective was to gather publicly available information about its domain registration, web technologies, DNS infrastructure, HTTP response headers, and Web Application Firewall (WAF).

The second activity involved using **Zenmap (Nmap GUI)** to scan my own local LAN, identify active hosts, examine their IP and MAC addresses, identify open ports and services, and visualize the network topology.

These exercises provided practical exposure to the initial stages of penetration testing and demonstrated how information gathering and network discovery contribute to security assessments.

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Operating system for reconnaissance activities |
| WHOIS | Retrieve domain registration information and name servers |
| WhatWeb | Identify website technologies, CMS and plugins |
| Nslookup | Resolve domain names to IP addresses |
| cURL | Inspect HTTP response headers |
| Wafw00f | Detect Web Application Firewalls |
| DNSRecon | Enumerate DNS records and infrastructure information |
| Zenmap | Discover live hosts, scan ports and visualize network topology |
| Windows CMD | Identify local IP address and network configuration |

---

## ⚙️ Tasks Completed

### 1. W2-PM1 – Multiple Kali Tools: Footprinting & Reconnaissance

Performed reconnaissance against `networkwalks.com` using six Kali Linux tools.

**Activities performed:**

- Retrieved publicly available domain registration information using WHOIS.
- Identified website technologies, including WordPress and WP Download Manager, using WhatWeb.
- Resolved the domain name to its IP address using Nslookup.
- Inspected HTTP response headers using cURL.
- Identified the Web Application Firewall using Wafw00f.
- Enumerated DNS records, including NS, MX, SPF/TXT and service-related records, using DNSRecon.

### 2. W2-PM5 – Zenmap: Network Scanning

Performed network discovery and port scanning on my own local LAN using Zenmap.

**Activities performed:**

- Used the Windows `ipconfig` command to identify my local IP address and subnet.
- Configured Zenmap with my local network subnet: `192.168.43.0/24`.
- Performed a network scan to identify active hosts.
- Identified two live hosts on the network.
- Examined IP and MAC addresses.
- Identified open ports and their associated services.
- Used the Topology tab to visualize the discovered network.
- Enabled and reviewed the topology legend.

---

## 🔍 Key Observations

### Footprinting & Reconnaissance

The reconnaissance activities revealed the following information:

| Finding | Observation |
|---|---|
| Domain | `networkwalks.com` |
| Server IP Address | `192.232.216.135` |
| CMS | WordPress 7.0.4 |
| Plugin | WP Download Manager 3.3.58 |
| Web Application Firewall | ModSecurity (SpiderLabs) |
| HTTP Information | Response headers and WordPress REST API endpoint |
| DNS Information | Name servers, mail servers and other DNS records |

### Network Scanning

The Zenmap scan identified two active hosts on my local network.

| IP Address | Open Ports | Identified Services |
|---|---|---|
| `192.168.43.1` | `53/tcp` | DNS |
| `192.168.43.131` | `135/tcp`, `139/tcp`, `445/tcp` | MSRPC, NetBIOS-SSN, Microsoft-DS |

The scan covered the `192.168.43.0/24` subnet and identified two active hosts out of 256 scanned IP addresses.

The results provided useful information about active devices, exposed ports and services within the local network.

---

## ⚠️ Risk Analysis & Recommendations

The practical exercises revealed several potential security observations:

| Observation | Potential Security Implication |
|---|---|
| Publicly exposed web technology information | Could assist attackers in identifying technologies for further investigation |
| Identifiable server IP address | Provides information about the hosting infrastructure |
| Exposed HTTP technical information | May assist technology fingerprinting and further enumeration |
| Identifiable WAF technology | Reveals information about the web application's security architecture |
| Publicly accessible DNS information | Helps build an infrastructure profile |
| Multiple active hosts and open ports | Highlights the importance of internal network monitoring |

### Recommendations

1. Regularly review publicly exposed website technology information.
2. Keep CMS platforms, plugins and web technologies updated.
3. Review HTTP response headers to minimize unnecessary information disclosure.
4. Regularly review DNS records and exposed services.
5. Properly configure and monitor Web Application Firewalls.
6. Perform regular internal network discovery.
7. Investigate unknown or unauthorized devices.
8. Maintain accurate network documentation and topology diagrams.
9. Conduct security testing only with appropriate authorization.

> **Note:** These observations represent potential security risks, not confirmed vulnerabilities. Further authorized security testing would be required to validate any actual vulnerabilities.

---

## 📸 Evidence & Documentation

This repository contains the practical evidence and documentation collected during the Week 2 project.

### Repository Contents

| Folder/File | Description |
|---|---|
| `Report/` | Contains the Week 2 Penetration Testing Report |
| `Evidence/` | Contains screenshots of the practical activities |
| `README.md` | Project overview, tools, activities and findings |

### Practical Evidence

The evidence includes:

- WHOIS domain registration results.
- WhatWeb technology fingerprinting results.
- Nslookup DNS resolution results.
- cURL HTTP response headers.
- Wafw00f detection results.
- DNSRecon enumeration results.
- Zenmap network scanning results.
- Network topology visualization.

📄 **[View Penetration Testing Report](Report/W2-PM-FINAL.pdf)**

📁 **[View Practical Evidence](Evidence/)**

---

## 🎓 What I Learned

This project strengthened my understanding of footprinting, reconnaissance and network scanning.

Through the Kali Linux tools, I gained practical experience gathering and interpreting publicly available information about a target domain and its web infrastructure.

Through Zenmap, I gained experience discovering active hosts, identifying open ports and running services, examining network information, and visualizing network topology.

I also learned the importance of:

- Interpreting technical outputs accurately.
- Identifying and documenting potential security risks.
- Providing appropriate security recommendations.
- Collecting evidence during security assessments.
- Conducting cybersecurity activities within an authorized scope.

Most importantly, I learned that identifying exposed information does not automatically mean a vulnerability exists. Proper validation and further authorized testing are necessary before drawing security conclusions.

---

## 🔐 Ethical Considerations

All activities were performed within the authorized scope:

- Domain reconnaissance was conducted with written permission.
- Network scanning was performed on my own local LAN.
- The practical exercises were conducted for educational and research purposes.
- No exploitation or unauthorized access was performed during these exercises.

---

## 🙏 Acknowledgment

This project was completed as part of the **NetworkWalks Cybersecurity Internship 2026**.

I appreciate NetworkWalks and the instructors for providing the opportunity to gain practical experience in cybersecurity and ethical hacking.

This repository documents my Week 2 practical activities, technical findings and learning progress.

Looking forward to building on these experiences as I continue developing my skills in cybersecurity and penetration testing.

---

**Author:** Uche Chimezie  
**Program:** NetworkWalks Cybersecurity Internship 2026  
**Project:** Week 2 – Footprinting & Network Scanning

**#Cybersecurity #EthicalHacking #PenetrationTesting #NetworkSecurity #KaliLinux #Nmap #Zenmap**
