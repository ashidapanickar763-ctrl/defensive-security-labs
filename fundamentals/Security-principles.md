# Security Principles for Defensive Security

## Overview

Security principles form the foundation of cybersecurity. Before learning tools such as Splunk, Wireshark, or Active Directory, it's important to understand the core concepts that guide how systems are designed, protected, and defended.

This document summarizes the fundamental security principles I studied while building my foundation for a career in defensive cybersecurity and SOC operations.

---

# Learning Objectives

- Understand the core principles of information security
- Learn how organizations protect systems and data
- Recognize common defensive security concepts
- Build a foundation for threat detection and incident response

---

# Topics Covered

## 1. CIA Triad

The CIA Triad is the foundation of information security.

### Confidentiality
Protects information from unauthorized access.

**Examples**
- Passwords
- Multi-Factor Authentication (MFA)
- Encryption
- Access Control

---

### Integrity

Ensures data remains accurate and unmodified.

**Examples**
- Hashing
- Checksums
- Digital Signatures
- File Integrity Monitoring

---

### Availability

Ensures systems and data remain accessible when needed.

**Examples**
- Backups
- Redundancy
- Load Balancing
- Disaster Recovery

---

## 2. Defense in Depth

Instead of relying on a single security control, organizations implement multiple layers of protection.

### Examples

- Firewall
- Antivirus
- IDS/IPS
- MFA
- SIEM
- Security Awareness Training

If one security layer fails, other controls continue protecting the environment.

---

## 3. Principle of Least Privilege (PoLP)

Users and applications should receive only the minimum permissions necessary to perform their tasks.

### Benefits

- Reduces attack surface
- Limits damage during compromise
- Prevents unauthorized access

---

## 4. Attack Surface

The attack surface includes every point where an attacker could attempt to gain access.

Examples include:

- Open network ports
- Public-facing web servers
- VPN gateways
- Email services
- User accounts
- Applications

Reducing unnecessary exposure decreases security risk.

---

## 5. Authentication vs Authorization

### Authentication

Verifies **who you are**.

Examples:
- Username & Password
- MFA
- Smart Cards
- Biometrics

---

### Authorization

Determines **what you are allowed to access** after authentication.

Examples:
- File permissions
- User roles
- Access Control Lists (ACLs)

---

## 6. Risk, Threat, and Vulnerability

### Asset

Something valuable to protect.

Examples:
- Servers
- User accounts
- Customer data

---

### Threat

Anything capable of causing harm.

Examples:
- Malware
- Phishing
- Insider threats
- Attackers

---

### Vulnerability

A weakness that can be exploited.

Examples:
- Unpatched software
- Weak passwords
- Misconfigurations

---

### Risk

The likelihood that a threat exploits a vulnerability.

---

# SOC Analyst Perspective

Security principles help SOC analysts:

- Understand why alerts occur
- Prioritize risks
- Reduce attack surface
- Investigate suspicious activity
- Recommend defensive controls
- Improve incident response decisions

---

# Key Takeaways

- Security starts with strong foundational principles.
- Layered security is more effective than relying on a single defense.
- Least privilege helps reduce potential damage during attacks.
- Understanding assets, threats, vulnerabilities, and risks improves security decision-making.

---

## 📌 Notes

This document is part of my **Defensive Security Labs** repository, where I document both my hands-on cybersecurity labs and the foundational concepts I'm learning while preparing for an entry-level SOC Analyst role.
