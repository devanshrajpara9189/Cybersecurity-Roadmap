# 🌐 Networking Ports

## 📌 Introduction

A **port** is a logical communication endpoint used by devices to identify specific services and applications on a network.

- Port range: **0 - 65535**
- Ports help multiple services run on the same device.
- Each service uses a specific port number.

---

# 📊 Port Categories

## 1. Well-Known Ports (0 - 1023)

These ports are assigned to common and widely used services.

---

| Port | Protocol | Full Form | Purpose |
|------|----------|-----------|---------|
| 20 | FTP | File Transfer Protocol | Transfers files (Data) |
| 21 | FTP | File Transfer Protocol | FTP command/control |
| 22 | SSH | Secure Shell | Secure remote login |
| 23 | Telnet | Teletype Network | Remote access (unencrypted) |
| 25 | SMTP | Simple Mail Transfer Protocol | Sending emails |
| 53 | DNS | Domain Name System | Converts domain names to IP addresses |
| 67 | DHCP | Dynamic Host Configuration Protocol | Provides IP addresses to clients (Server) |
| 68 | DHCP | Dynamic Host Configuration Protocol | Receives IP addresses (Client) |
| 80 | HTTP | Hypertext Transfer Protocol | Web communication |
| 110 | POP3 | Post Office Protocol v3 | Email receiving |
| 143 | IMAP | Internet Message Access Protocol | Email synchronization |
| 443 | HTTPS | Hypertext Transfer Protocol Secure | Secure web communication |

---

# 🔐 Important Secure Ports

| Port | Protocol | Purpose |
|------|----------|---------|
| 22 | SSH | Encrypted remote access |
| 443 | HTTPS | Secure websites |
| 465 | SMTPS | Secure email sending |
| 993 | IMAPS | Secure email receiving |
| 995 | POP3S | Secure email receiving |

---

# 🖥️ Common Additional Ports

| Port | Protocol | Purpose |
|------|----------|---------|
| 3389 | RDP | Remote Desktop Protocol |
| 445 | SMB | File and printer sharing |
| 139 | NetBIOS | Windows network services |
| 161 | SNMP | Network monitoring |
| 162 | SNMP Trap | Network alerts |
| 389 | LDAP | Directory services |
| 636 | LDAPS | Secure LDAP |
| 3306 | MySQL | Database service |
| 5432 | PostgreSQL | Database service |
| 1433 | MSSQL | Microsoft SQL Server |
| 5900 | VNC | Remote desktop access |
| 8080 | HTTP Proxy | Alternative web service port |

---

# 📂 Port Classes

## Registered Ports (1024 - 49151)

Used by applications and software vendors.

Examples:

- Database services
- Applications
- Development tools

---

## Dynamic / Private Ports (49152 - 65535)

Used temporarily by client applications.

Examples:

- Temporary connections
- User applications

---

# 🛡️ Security Importance of Ports

Security professionals analyze ports to:

- Identify running services
- Find unnecessary open ports
- Detect vulnerabilities
- Configure firewalls

Example:

Open port 22 → SSH service running  
Open port 80 → Web server running

---

# 🔍 Port Scanning

Port scanning is used to identify open ports and services on a system.

Common security tool:

- Nmap

Purpose:

- Network discovery
- Security assessment
- Vulnerability identification

---

# ⭐ Key Concept

**IP Address identifies the device.**  
**Port number identifies the service running on that device.**

Example:
192.168.1.10:443 

IP Address → Device  
Port 443 → HTTPS Service


This will fit under your Networking Fundamentals module and is useful for SOC, CEH, eJPT, and OSCP basics.
