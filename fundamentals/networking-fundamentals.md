# Networking Fundamentals for Defensive Security

## Overview

As part of my SOC Analyst learning journey, I studied the core networking concepts that form the foundation of defensive security.

Understanding how devices communicate, how traffic flows across a network, and how common protocols work is essential before learning topics such as SIEM, log analysis, threat detection, and incident response.

This document summarizes the networking concepts I learned while building my cybersecurity foundation.

---

#  Learning Objectives

- Understand how network communication works
- Learn common protocols and their purposes
- Identify commonly used network ports
- Understand how security devices protect networks
- Learn how DNS resolves domain names
- Build a strong foundation for SOC investigations

---

# Topics Covered

## 1. OSI Model

The OSI (Open Systems Interconnection) model explains how data travels between devices across a network.

### Seven Layers

| Layer | Name | Purpose |
|--------|------|---------|
| 7 | Application | User-facing applications |
| 6 | Presentation | Data formatting and encryption |
| 5 | Session | Establishes and manages sessions |
| 4 | Transport | Reliable communication (TCP/UDP) |
| 3 | Network | IP addressing and routing |
| 2 | Data Link | MAC addresses and switching |
| 1 | Physical | Cables, signals, and hardware |

---

## 2. TCP/IP Model

The TCP/IP model is the practical networking model used on modern networks.

| Layer | Purpose |
|--------|----------|
| Application | Network applications |
| Transport | TCP and UDP communication |
| Internet | IP routing |
| Network Access | Physical network communication |

---

## 3. Common Network Ports

| Port | Protocol | Purpose |
|------|-----------|----------|
| 21 | FTP | File Transfer |
| 22 | SSH | Secure Remote Login |
| 23 | Telnet | Remote Login (Insecure) |
| 25 | SMTP | Email Transfer |
| 53 | DNS | Name Resolution |
| 80 | HTTP | Web Traffic |
| 443 | HTTPS | Secure Web Traffic |
| 445 | SMB | Windows File Sharing |
| 161 | SNMP | Network Monitoring |
| 3389 | RDP | Remote Desktop |
| 3306 | MySQL | Database Service |

---

## 4. Security Devices

### Firewall
Filters incoming and outgoing network traffic based on security rules.

### IDS
Detects suspicious or malicious activity and generates alerts.

### IPS
Detects and actively blocks malicious traffic.

### Proxy
Acts as an intermediary between users and servers.

### VPN
Creates an encrypted tunnel to securely transmit data.

---

## 5. DNS Resolution Flow

Understanding DNS resolution is important because attackers often target DNS infrastructure.

### Steps

1. User enters a domain name
2. Browser checks local cache
3. Request goes to Recursive Resolver
4. Resolver contacts Root Server
5. Root Server refers to TLD Server
6. TLD Server refers to Authoritative Name Server
7. Authoritative Server returns the IP address
8. Browser connects to the destination server

---

### 6. DHCP Concepts
DHCP automatically assigns an IP address to a device when it joins a network, instead of requiring manual configuration. This happens through a 4-step process known as **DORA**:
- **Discover** — device asks if any DHCP server is available
- **Offer** — DHCP server offers an available IP address
- **Request** — device requests that specific IP address
- **Acknowledge** — DHCP server confirms and assigns the IP

### 7. Cisco Packet Tracer (Practical Exercises)
Completed hands-on VLAN, routing, and DHCP/DNS configuration exercises during diploma coursework — building and testing small network topologies to see these concepts working in practice rather than just in theory.
# SOC Analyst Perspective

Networking knowledge helps SOC analysts:

- Investigate suspicious traffic
- Understand firewall alerts
- Analyze DNS requests
- Detect unusual network behavior
- Identify exposed services
- Interpret packet captures
- Correlate security events

---

# Key Takeaways

- Networking is the foundation of cybersecurity.
- Every defensive security tool relies on networking concepts.
- Understanding protocols and ports makes security alerts easier to investigate.
- DNS and network traffic analysis are essential skills for SOC analysts.

---

## My Learning Reflection

Before studying networking, I mainly focused on learning cybersecurity tools. This topic helped me understand that every security alert, packet capture, and SIEM event is built on networking fundamentals.

Learning concepts such as the OSI model, common ports, DNS resolution, and network security devices gave me a much clearer understanding of how systems communicate and how SOC analysts investigate network-based threats.

This foundation will support my future learning in Splunk, Windows Event Logs, Wireshark, Active Directory, and incident response.

##  Notes

This document is part of my **Defensive Security Labs** repository, where I document my hands-on labs and foundational cybersecurity learning as I work toward becoming an entry-level SOC Analyst.
