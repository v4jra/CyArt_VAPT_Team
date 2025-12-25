# Environment Setup & Tool Configuration

## Overview
This directory documents the complete setup used during Week-4 of the VAPT internship project. All tools and environments were configured locally to simulate real-world penetration testing conditions.

---

## Operating System
- Kali Linux (Attacker Machine)
- VulnHub / Metasploitable 2 (Target Machines)
- Android APK Analysis (Offline)

---

## Virtualization Setup
- VirtualBox
- Network Mode: Host-Only / Internal Network
- IP Allocation: Static / DHCP (Lab-based)

---

## Tool Setup Details

### Kali Linux (Native Installation)
The following tools were used directly from Kali repositories:
- Metasploit Framework
- Nmap
- Burp Suite Community
- sqlmap
- Responder
- Ettercap
- Wireshark
- mitmproxy
- LinPEAS
- PowerSploit

---

### Docker-Based Setup
Docker was used for tools requiring isolated environments.

#### MobSF (Mobile Security Framework)
- Deployment: Docker
- Purpose: Static & Dynamic Android Application Analysis
- Output: PDF reports (stored in `/reports/mobsf/`)

---

### Ghidra Setup
- Used for static binary analysis
- Imported vulnerable binaries
- Analyzed unsafe functions and memory flow

---

## Network Configuration
- Host-Only networking enabled
- Attacker and victim in same subnet
- IP forwarding enabled for MitM attacks

---

## Notes
- All tools were used in authorized lab environments only
- No production systems were targeted
