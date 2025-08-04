# network-port-scan-task
scan_result.txt – Nmap scan output

README.md – Short explanation (template below)

services_and_risks.md – Table of open ports, services, and security concerns

# 🔐 Task 1 – Local Network Port Scanning (Cyber Security Internship)

## 📌 Objective
To discover open ports in a local network using **Nmap**, understand what services are exposed, and identify potential security risks.

---

## 🛠 Tools Used
- **Nmap** – Port scanning and network reconnaissance tool
- (Optional) Wireshark – For traffic analysis (not used in this task)

---

## 🌐 Network Details
- **IP Range Scanned:** 192.168.1.0/24
- **Target Device IP:** 192.168.1.15

---

## 🧪 Command Used
```bash
nmap -sS 192.168.1.0/24 -oN scan_result.txt
