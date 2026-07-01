# Common Attacks

## Overview

Understanding common cyber attacks is essential for detecting, investigating, and responding to security incidents. 
This section documents my learning of frequently encountered attack techniques from a defender's perspective.

Summary

Covers 4 attack categories: Social Engineering, Malware, Network Attacks, Password Attacks. 
This room is concept-based rather than lab-based — just building the attack vocabulary I'll use in later hands-on rooms.

Attack Types — Quick Reference

Type                   Examples                           How It Works   
Social Engineering     Phishing, pretexting,baiting       Targets people,not systems
Malware                Virus, worm, trojan, ransomware    Differ by propagation method 
Network Attacks        DoS/DDoS, MITM                     Disrupt or intercept communication
Password Attacks       Brute force, dictionary,           Differ by method of guessing/reusing
                          credential stuffing                              credentials            

Where Each Attack Shows Up (Detection Surface)

Attack                     Log/Source to Check
Phishing                   Email gateway logs 
Malware                    EDR/AV logs
DoS/DDoS                   Firewall logs, NetFlow 
MITM                       ARP tables, DNS logs
Brute force                Auth logs (e.g. Event ID 4625)

One Thing I Took Away

Before this room I treated "social engineering" and "phishing" as the same thing.
Now I know phishing is just one method under the broader social engineering category — the room made that distinction clear with simple examples.

Key terms


T1566 – Phishing
T1110 – Brute Force
T1557 – Adversary-in-the-Middle
T1498 – Network Denial of Service
Event ID 4625 – Failed logon attempt

> **Note:** This repository focuses on defensive learning and documentation. It does not contain exploit code, challenge solutions, or walkthroughs.
