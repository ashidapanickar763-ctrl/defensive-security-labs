# Common Attacks

## Overview

Understanding common cyber attacks is essential for detecting, investigating, and responding to security incidents. 
This section documents my learning of frequently encountered attack techniques from a defender's perspective.

Summary

Covers 4 attack categories: Social Engineering, Malware, Network Attacks, Password Attacks. 
This room is concept-based rather than lab-based — just building the attack vocabulary I'll use in later hands-on rooms.

Attack Types — Quick Reference

| Attack Type | Examples | How It Works | Detection Sources |
|-------------|----------|--------------|-------------------|
| Social Engineering | Phishing, Pretexting, Baiting | Tricks people into revealing information | Email Gateway Logs, User Reports |
| Malware | Virus, Worm, Trojan, Ransomware | Malicious software infects systems | EDR Logs, Antivirus Alerts |
| Network Attacks | DoS, DDoS, MITM | Disrupts or intercepts network traffic | Firewall Logs, NetFlow, DNS Logs |
| Password Attacks | Brute Force, Dictionary, Credential Stuffing | Attempts to gain unauthorized access | Windows Event ID 4625, Authentication Logs |

---
## Detection Tips

- **Email Gateway Logs** → Detect phishing emails.
- **EDR Logs** → Detect malware execution.
- **Firewall Logs** → Detect DoS/DDoS activity.
- **Windows Event ID 4625** → Detect failed logon attempts.

---

## Where Each Attack Shows Up (Detection Surface)

| Attack | Log/Source to Check |
|--------|----------------------|
| Phishing | Email Gateway Logs |
| Malware | EDR/AV Logs |
| DoS/DDoS | Firewall Logs, NetFlow |
| MITM | ARP Tables, DNS Logs |
| Brute Force | Authentication Logs (Windows Event ID 4625) |

Before this room I treated "social engineering" and "phishing" as the same thing.
Now I know phishing is just one method under the broader social engineering category — the room made that distinction clear with simple examples.

## Key MITRE ATT&CK Techniques

- T1566 – Phishing
- T1110 – Brute Force
- T1557 – Adversary-in-the-Middle
- T1498 – Network Denial of Service

---
> **Note:** This repository focuses on defensive learning and documentation. It does not contain exploit code, challenge solutions, or walkthroughs.
