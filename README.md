# 🔐 Cybersecurity Home Lab
### Penetration Testing & Vulnerability Assessment — Metasploitable 2

> A self-initiated cybersecurity project built to develop practical offensive and defensive security skills. All activity was conducted in a fully isolated virtual lab environment on my own machines for educational purposes only.

---

## 📌 Project Summary

As part of my preparation for a career in cybersecurity, I built a virtual home lab from scratch and conducted a full penetration test against a deliberately vulnerable target machine. This project covers the complete lifecycle of a security assessment from reconnaissance through to exploitation, detection, and remediation documented to a professional standard.

---

## 🖥️ Lab Environment

| Component | Details |
|---|---|
| Virtualisation Platform | Oracle VirtualBox |
| Attacker Machine | Kali Linux (rolling release) |
| Target Machine | Metasploitable 2 |
| Network Type | VirtualBox Internal Network (fully isolated) |
| Attacker IP | 192.168.56.20 |
| Target IP | 192.168.56.10 |

Both machines were configured on an isolated internal network with no external internet exposure, ensuring no risk to live systems at any point.

---

## 🎯 Project Objectives

- Build and configure a safe, isolated virtual lab network from scratch
- Perform network reconnaissance to identify open ports, services, and vulnerabilities
- Exploit known CVEs in a controlled environment using industry-standard tools
- Extract and analyse password hashes to demonstrate credential security risks
- Analyse system logs to identify evidence of intrusion from a defender's perspective
- Apply firewall rules and service hardening to remediate identified vulnerabilities
- Document all findings to a professional penetration testing report standard

---

## 🔍 Vulnerabilities Identified

| # | Vulnerability | CVE | Port / Service | Risk Rating | Remediated |
|---|---|---|---|---|---|
| 1 | Samba usermap_script | CVE-2007-2447 | 445 / SMB | 🔴 Critical | ✅ Yes |
| 2 | vsftpd 2.3.4 Backdoor | CVE-2011-2523 | 21 / FTP | 🔴 Critical | ✅ Yes |
| 3 | Weak Password Storage | N/A | System | 🟠 High | ✅ Yes |
| 4 | Telnet Service Exposed | N/A | 23 / Telnet | 🟠 High | ✅ Yes |
| 5 | Outdated OpenSSH | N/A | 22 / SSH | 🟡 Medium | ✅ Yes |
| 6 | MySQL Exposed on Network | N/A | 3306 / MySQL | 🟠 High | ✅ Yes |
| 7 | VNC No Encryption | N/A | 5900 / VNC | 🟠 High | ✅ Yes |

---

## 🧰 Tools Used

| Tool | Purpose |
|---|---|
| nmap | Network scanning, port enumeration, service and OS detection |
| Metasploit Framework | Vulnerability exploitation and post-exploitation |
| John the Ripper | Password hash cracking and credential analysis |
| iptables | Firewall rule configuration for remediation |
| Netcat | Manual exploit triggering and connection testing |
| Kali Linux CLI | System exploration, log analysis, post-exploitation |

---

## 📋 Full Report

The complete penetration test report is available here:

👉 [View Full Report](reports/metasploitable-pentest-report.md)

The report covers:
- Detailed reconnaissance findings
- Step-by-step exploitation walkthroughs
- Post-exploitation analysis
- Blue team log analysis and detection
- Full remediation steps with verification
- Risk ratings and recommended long-term fixes

---

## 📸 Screenshots

Evidence screenshots are stored in the screenshots folder, including:
- nmap scan output showing all open ports and services
- Successful root shell access
- Password hash extraction from /etc/shadow
- John the Ripper cracking output
- Remediation verification (failed exploit attempts post-fix)

---

## 💡 What I Learned

- How attackers perform systematic reconnaissance before targeting specific services
- How well-known CVEs work in practice and why unpatched software is dangerous
- How to read system logs and identify indicators of compromise
- How firewall rules and service hardening significantly reduce attack surface
- How to document security findings to a professional report standard
- The importance of strong password policies and secure credential storage

---

## 🔗 Relevant CVE References

- [CVE-2007-2447 — Samba usermap_script](https://nvd.nist.gov/vuln/detail/CVE-2007-2447)
- [CVE-2011-2523 — vsftpd 2.3.4 Backdoor](https://nvd.nist.gov/vuln/detail/CVE-2011-2523)

---

## ⚠️ Disclaimer

All activity documented in this project was performed in a fully isolated virtual lab environment on my own personal machines, for educational purposes only. No real systems, networks, or third-party infrastructure were targeted at any point. This project is intended solely to demonstrate practical cybersecurity skills for career development.
