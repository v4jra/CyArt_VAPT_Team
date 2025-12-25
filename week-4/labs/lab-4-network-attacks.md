# Lab 4 – Network Protocol Attacks

## Objective
To demonstrate Man-in-the-Middle (MitM) attacks and insecure protocol exploitation.

---

## Scope
- SMB protocol attacks
- ARP spoofing
- Credential interception

---

## Tools Used
- Responder
- Ettercap
- Wireshark
- mitmproxy

---

## Attack Simulation

| Attack ID | Technique | Target | Status | Outcome |
|---------|----------|--------|--------|--------|
| 015 | SMB Relay Attack | Lab VM | Success | NTLM Hash Captured |

---

## Practical Case – mitmproxy
During a controlled lab exercise, mitmproxy was used to intercept HTTP/HTTPS traffic. Sensitive credentials were observed due to improper transport security.

---

## Impact
Captured credentials demonstrated risks associated with insecure network configurations.

---

## Recommendations
- Enable SMB signing
- Use encrypted communication
- Implement network segmentation
