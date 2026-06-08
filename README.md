# CyberSecurity-Home-Lab
Cybersecurity Home Lab — Penetration Testing & Vulnerability Assessment

## Overview
A self-initiated cybersecurity project where I built an isolated virtual 
lab environment to practice ethical hacking and defensive security techniques.
This project was undertaken to develop practical skills in preparation for 
a career in cybersecurity.

---

## 🛠️ Lab Environment
| Component | Details |
|---|---|
| Virtualisation Platform | Oracle VirtualBox |
| Attacker Machine | Kali Linux |
| Target Machine | Metasploitable 2 |
| Network | Isolated Internal Network (no internet exposure) |

---

## 🎯 Objectives
- Build and configure a safe, isolated virtual network
- Perform network reconnaissance to identify vulnerabilities
- Exploit known CVEs in a controlled environment
- Analyse system logs to detect attack evidence
- Apply remediations and verify effectiveness
- Document findings in a professional security report

---

## 🔍 Vulnerabilities Found
| Vulnerability | CVE | Port | Risk Rating | Status |
| Samba usermap_script | CVE-2007-2447 | 445 | Critical | Remediated |
| vsftpd 2.3.4 Backdoor | CVE-2011-2523 | 21 | Critical | Remediated |
| Weak Password Storage | N/A | N/A | High | Remediated |

---

## 🧰 Tools Used
- **nmap** — network scanning and service enumeration
- **Metasploit Framework** — vulnerability exploitation
- **John the Ripper** — password hash cracking
- **iptables** — firewall rule configuration
- **Netcat** — manual exploit triggering

---

## 📋 Reports
- [Full Penetration Test Report](reports/metasploitable-pentest-report.md)

---

## 🔵 What I Learned
- How attackers perform reconnaissance before exploiting systems
- How known CVEs work in practice and why patching is critical
- How to read and analyse system logs to detect intrusions
- How firewall rules and service hardening reduce attack surface
- How to document findings professionally in a pentest report format

---

## ⚠️ Disclaimer
All activity was performed in a fully isolated virtual lab environment 
on my own machines for educational purposes only. No real systems were 
targeted at any point.
