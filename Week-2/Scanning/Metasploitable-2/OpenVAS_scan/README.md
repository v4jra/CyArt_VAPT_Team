
# OpenVAS / Greenbone Vulnerability Scanning

This folder contains all vulnerability scanning results performed using **OpenVAS (Greenbone Vulnerability Manager)**.  
All reports, CVE references, and screenshots are organized for professional VAPT documentation.

---

# 1. Objective

OpenVAS was used to identify:

- **High-risk vulnerabilities**
- **Outdated software versions**
- **Misconfigurations**
- **Network-exposed services**
- **CVE-mapped security issues**

The goal of this scan is to **prioritize risk** and provide **actionable remediation steps**.

---

# 2. Scan Configuration

### Scan Type  
- Full & Fast  
- Authenticated (where possible)  
- Network discovery enabled  
- Default scripts + CVE feed update

### Target Machines  
- **Metasploitable 2**
- **DVWA (Docker – Port 9988)**

### Feed Update Command (Used if required)

```bash
sudo greenbone-feed-sync
