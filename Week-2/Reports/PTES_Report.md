# PTES VAPT Report – Week 2 Assessment (200 Words)

This assessment followed the PTES methodology, covering reconnaissance, scanning, exploitation, and post-exploitation phases. Initial reconnaissance using Shodan identified exposed ProFTPD and Postfix SMTP services, revealing outdated versions and publicly visible banners, indicating attack exposure.  

During scanning, Nmap and OpenVAS were used on DVWA and Metasploitable2 environments. The scans revealed multiple high-risk vulnerabilities including SQL Injection, Cross-Site Scripting (XSS), Local File Inclusion (LFI), OS Command Injection, and misconfigured file upload functionalities.

In the exploitation phase, sqlmap validated SQL injection vulnerabilities on DVWA, while Burp Suite confirmed XSS, command injection, and insecure upload flaws. On Metasploitable2, Metasploit successfully exploited the Tomcat Manager resulting in remote code execution. The obtained shell allowed further enumeration such as user discovery, network information gathering, and configuration inspection. Hash-based integrity checks were also performed for evidence collection.

Privilege escalation was not required since the exploited service provided direct root-level access. Post-exploitation included analyzing service configurations, reviewing system architecture, and documenting evidence.

The overall security posture is rated high-risk. Immediate remediation is recommended, including patching outdated services, enforcing strict input validation, disabling unnecessary ports, and re-scanning after fixes.

All findings are documented with screenshots and tool outputs.
