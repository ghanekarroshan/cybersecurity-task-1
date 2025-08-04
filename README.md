Cyber Security Internship - Task 1

Task: Scan Your Local Network for Open Ports

Description
This project is part of my Cyber Security Internship. The goal of this task was to scan a local network to identify open ports on connected devices using "Nmap". This process helps understand the basic concepts of network reconnaissance, open port vulnerabilities, and securing network services.

---

Tools Used
- "Nmap" – For network scanning and port discovery
- "Kali Linux" – (or any terminal-supported OS)


---

Command Used
```bash
nmap -sS -oX scan_results.xml 192.168.146.0/24
-sS: TCP SYN scan (stealth scan)

-oX: Output in XML format (later converted to HTML)

Scan Summary
IP Range Scanned: 192.168.146.0/24

Devices Found Online: 4

Scan Duration: 8.67 seconds

Open Ports Found: 1 (Port 53 on one device)

Devices Detected

| IP Address      | Status | Open Ports | Service            |
| --------------- | ------ | ---------- | ------------------ |
| 192.168.146.1   | Online | None       | All ports filtered |
| 192.168.146.2   | Online | 53/tcp     | DNS (domain)       |
| 192.168.146.128 | Online | None       | All ports closed   |
| 192.168.146.254 | Online | None       | All ports filtered |


Security Observations
Port 53/tcp (DNS) open on 192.168.146.2. This may indicate a DNS service is active.

Other hosts appear secure with all ports either closed or filtered.

No suspicious or risky services detected in this scan.

Files Included
scan_results.html – Human-readable Nmap scan output

README.md – Summary, commands used, and observations

Key Takeaways
Learned how to perform a TCP SYN scan using Nmap.

Understood how to interpret open/closed/filtered ports.

Gained insight into network exposure and the importance of minimizing open ports.

Author
Roshan Ghanekar – Cyber Security Intern
Date :- 04/08/2025