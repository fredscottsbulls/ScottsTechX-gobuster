# \U0001F47B ScottsTechX Gobuster

<p align="center">
  <img src="https://img.shields.io/badge/Gobuster-Directory-Buster-00ff88?style=for-the-badge&logo=linux&logoColor=black" alt="Gobuster"/>
  <img src="https://img.shields.io/badge/Web-Security-00ff88?style=for-the-badge&logo=shield&logoColor=black" alt="Web Security"/>
</p>

> **Directory/file discovery, DNS subdomains, and virtual host enumeration.**

---

## \u26A1 What It Does

Gobuster discovers hidden paths, directories, files, subdomains, and virtual hosts on web servers \u2014 essential for web application reconnaissance.

## \U0001F680 Quick Usage

```bash
# Directory busting
gobuster dir -u http://target.com -w wordlist.txt

# DNS subdomain enumeration
gobuster dns -d target.com -w subdomains.txt

# Virtual host discovery
gobuster vhost -u http://target.com -w subdomains.txt

# File extension scan
gobuster dir -u http://target.com -w wordlist.txt -x php,html,js
```

## \U0001F6E1 Bug Bounty Workflow

```bash
gobuster dir -u https://target.com -w /usr/share/wordlists/dirb/common.txt -t 50
gobuster dns -d target.com -w /usr/share/wordlists/subdomains.txt
gobuster vhost -u https://target.com -w /usr/share/wordlists/subdomains.txt
```

---

MIT \u00a9 2026
