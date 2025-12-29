# Week-1 : Vulnerability Assessment & Penetration Testing (VAPT)

## Project Title
Vulnerability Assessment & Penetration Testing on Born2Root VM

## Author
**Alok Kumar Sahu**

## Week
**Week-1**

## Environment Overview
This project focuses on performing Vulnerability Assessment and Penetration Testing (VAPT) on a vulnerable virtual machine using industry-standard open-source tools.

Due to system RAM limitations, **Metasploitable 3** could not be used. Instead, **Born2Root VM** was selected as the target, which provides similar vulnerable configurations for effective security testing.

---

## Objective
- Identify vulnerabilities in the target system  
- Analyze risk severity using CVSS scores  
- Document findings with evidence  
- Suggest remediation steps following security best practices  

---

## Tools Used

| Tool Name | Purpose |
|---------|--------|
| Kali Linux | Attacker Machine |
| Nmap | Network scanning & service enumeration |
| OpenVAS | Vulnerability assessment |
| Nikto | Web server vulnerability scanning |
| Born2Root VM | Target vulnerable machine |

---

## Virtual Machines Used

| Role | OS / VM |
|----|--------|
| Attacker | Kali Linux |
| Target | Born2Root VM |
| Target IP | `212.83.142.84` |

---

## Methodology Followed (VAPT Phases)

1. **Planning**
   - Target identification
   - Tool selection

2. **Discovery**
   - Port scanning (Nmap)
   - Vulnerability scanning (OpenVAS)
   - Web scanning (Nikto)

3. **Attack / Analysis**
   - Identification of misconfigurations
   - Risk assessment using CVSS

4. **Reporting**
   - Documentation of vulnerabilities
   - Screenshots & tool outputs
   - Remediation suggestions

---

## Vulnerabilities Identified

| ID | Vulnerability | Service | Risk Level | CVSS |
|---|--------------|--------|-----------|------|
| V-01 | OS End of Life (EOL) | System | High | 10.0 |
| V-02 | Weak SSH Host Key Algorithms | SSH | Medium | 6.4 |
| V-03 | HTTP Directory Indexing Enabled | Apache | Medium | 5.3 |

---

## Vulnerability Details

### 1. OS End of Life (EOL)
- **Description:** Target system is running an unsupported Debian OS
- **Risk:** No security patches available
- **Remediation:** Upgrade to a supported OS version

### 2️. Weak SSH Host Key Algorithms
- **Description:** Weak cryptographic algorithms enabled in SSH
- **Risk:** Susceptible to cryptographic attacks
- **Remediation:** Use ECDSA or ED25519 keys and disable weak algorithms

### 3️. HTTP Directory Indexing
- **Description:** Apache server allows directory listing
- **Risk:** Exposure of sensitive files
- **Remediation:** Disable directory indexing using `Options -Indexes`

---

## Files & Evidence Included
- `openvas_scan_report.xml`
- `nmap_scan_report.txt`
- `nikto_scan_report.txt`
- Screenshots of vulnerabilities

---

## Key Learnings
- Practical experience with OpenVAS, Nmap, and Nikto  
- Understanding CVSS-based risk assessment  
- Importance of OS patching and secure configurations  
- Hands-on exposure to VAPT lifecycle  

---

## References
- Nmap: https://nmap.org  
- OpenVAS: https://www.openvas.org  
- Nikto: https://cirt.net/Nikto2  
- CVE Database: https://cve.mitre.org  

---

## ✅ Conclusion
This Week-1 VAPT assessment successfully identified critical and medium-risk vulnerabilities in the Born2Root VM. Proper remediation such as OS upgrades, secure SSH configurations, and hardened web server settings are strongly recommended to improve system security.

---

