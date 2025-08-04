This performs a TCP SYN scan over the local network and saves results to a text file.

🔍 Scan Result Summary
✔️ Device Found: 192.168.1.15
Port	State	Service	Description
| Port | State | Service      | Description                                                                  |
| ---- | ----- | ------------ | ---------------------------------------------------------------------------- |
| 135  | open  | msrpc        | Microsoft RPC service; used internally by Windows; can be exploited remotely |
| 139  | open  | netbios-ssn  | NetBIOS Session Service; used for file sharing; often targeted in attacks    |
| 445  | open  | microsoft-ds | SMB service; used for Windows file sharing and Active Directory              |
| 5357 | open  | wsdapi       | Web Services for Devices; typically for printers and media devices           |


⚠️ Security Risk Analysis
Ports 135, 139, and 445 are well-known for being vulnerable to attacks like malware (e.g., WannaCry ransomware).

These should be firewalled or disabled if not required, especially on publicly exposed systems.

Port 5357 (WSDAPI) is generally safe on local networks but should still be monitored.

📁 Files in This Repo
scan_result.txt – Full raw output from Nmap

services_and_risks.md – List of open ports, services, and associated risks

README.md – This file, explaining the task and outcomes

✅ Outcome
Understood how to use Nmap for port scanning

Learned about common Windows network services and their vulnerabilities

Practiced basic network reconnaissance and security risk assessment

