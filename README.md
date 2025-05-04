# Create a simple progress badge in Markdown format using shields.io

# Total tasks completed: 3 (based on previously added labs)
# Estimated total items in the roadmap (customizable): 25
completed = 3
total = 25
percentage = int((completed / total) * 100)

# Construct badge URL using shields.io
badge_url = f"https://img.shields.io/badge/Progress-{percentage}%25-brightgreen"

# Generate markdown snippet for the badge
badge_markdown = f"![Progress Badge]({badge_url})\n\n> **Training Progress**: {completed} of {total} tasks complete ({percentage}%)"

badge_markdown

# 🛡️ Ethical Hacking Training Plan

## 🎯 Objective
Build foundational and advanced ethical hacking skills through structured, progressive hands-on learning.

---

## 🧱 1. Foundations: Lab & Basics
- [x] Kali Linux installed
- [x] Metasploitable 2 configured
- [ ] Networking basics
- [ ] Kali terminal skills

## 🔧 2. Recon & Scanning
- [ ] [Nmap scanning basics](labs/nmap-basics.md)
- [ ] Gobuster and Nikto
- [ ] Service detection

## 💣 3. Exploitation
- [ ] [FTP exploit (vsftpd 2.3.4)](labs/ftp-vsftpd.md)
- [ ] [Telnet brute-force](labs/telnet-login.md)
- [ ] Metasploit framework basics


## 🧬 4. Post-Exploitation
- [ ] Shell interaction
- [ ] Privilege escalation
- [ ] Persistence tactics

## 🌐 5. Web App Hacking
- [ ] SQLi, XSS, CSRF via DVWA or Mutillidae

## 🧠 6. Advanced Topics
- [ ] AD exploitation
- [ ] OSINT & Red teaming
- [ ] Buffer overflows

## 📋 7. Certifications & Goals
- [ ] CEH / eJPT / PNPT
- [ ] Hack The Box
- [ ] TryHackMe Paths

---
This repository is your roadmap to mastering ethical hacking. Document your journey in `/notes`, practice in `/labs`, and track progress in `/checklists`.
