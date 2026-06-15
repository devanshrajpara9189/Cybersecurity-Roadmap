# 🌐 Network Protocols

## 📌 Introduction

A **network protocol** is a set of rules that defines how devices communicate and exchange data over a network.

Protocols define:

- How data is transmitted
- How devices identify each other
- How errors are handled
- How communication is secured

---

# 📚 Types of Network Protocols

## 🔹 HTTP (Hypertext Transfer Protocol)

Port: **80**

Purpose:

- Transfers web pages between browser and web server
- Used for normal web communication

Example:
http://website.com 


---

## 🔒 HTTPS (Hypertext Transfer Protocol Secure)

Port: **443**

Purpose:

- Secure version of HTTP
- Encrypts communication using TLS/SSL

Provides:

- Confidentiality
- Integrity
- Authentication

Example:
https://website.com


---

## 📂 FTP (File Transfer Protocol)

Ports:

- 20 → Data transfer
- 21 → Control connection

Purpose:

- Transfers files between systems

Security issue:

- Data is transferred without encryption

---

## 🔐 SFTP (Secure File Transfer Protocol)

Port: **22**

Purpose:

- Secure file transfer using SSH encryption

Benefits:

- Encrypted communication
- Secure authentication

---

## 🖥️ SSH (Secure Shell)

Port: **22**

Purpose:

- Secure remote login
- Remote system administration

Features:

- Encryption
- Secure command execution

---

## 📧 SMTP (Simple Mail Transfer Protocol)

Port:

- 25
- 587 (secure email submission)

Purpose:

- Sending emails between mail servers

---

## 📩 POP3 (Post Office Protocol Version 3)

Port:

- 110
- 995 (secure)

Purpose:

- Downloads emails from server to device

---

## 📬 IMAP (Internet Message Access Protocol)

Port:

- 143
- 993 (secure)

Purpose:

- Synchronizes emails between server and devices

---

## 🌍 DNS (Domain Name System)

Port:

- 53

Purpose:

- Converts domain names into IP addresses

Example:
google.com → IP Address


---

## 📡 DHCP (Dynamic Host Configuration Protocol)

Ports:

- 67 (Server)
- 68 (Client)

Purpose:

Automatically provides:

- IP address
- Subnet mask
- Default gateway
- DNS information

---

## 🔗 TCP (Transmission Control Protocol)

Purpose:

- Reliable data communication

Features:

- Connection-oriented
- Error checking
- Data delivery confirmation

Examples:

- HTTP
- HTTPS
- SSH

---

## ⚡ UDP (User Datagram Protocol)

Purpose:

- Fast data transmission

Features:

- Connectionless
- No delivery guarantee
- Lower delay

Examples:

- DNS
- Online gaming
- Video streaming

---

# 🛡️ Security Protocols

## 🔐 TLS (Transport Layer Security)

Purpose:

- Encrypts communication over networks

Used in:

- HTTPS
- Secure emails
- VPNs

---

## 🔑 IPsec (Internet Protocol Security)

Purpose:

- Provides secure IP communication

Used in:

- VPN connections

---

## 🔒 SSL (Secure Sockets Layer)

Purpose:

- Older encryption protocol replaced by TLS

---

# 🖥️ Remote Access Protocols

## RDP (Remote Desktop Protocol)

Port: **3389**

Purpose:

- Remote access to Windows systems

---

## Telnet

Port: **23**

Purpose:

- Remote login

Security issue:

- Data is transmitted without encryption

---

# 📊 Network Management Protocols

## SNMP (Simple Network Management Protocol)

Ports:

- 161 → Monitoring
- 162 → Alerts

Purpose:

- Network device monitoring
- Collecting device information

---

# 📁 File Sharing Protocols

## SMB (Server Message Block)

Port:

- 445

Purpose:

- File and printer sharing in Windows networks

---

## NFS (Network File System)

Purpose:

- File sharing between Linux/Unix systems

---

# 🌐 Routing Protocols

## RIP (Routing Information Protocol)

Purpose:

- Finds routes between networks

---

## OSPF (Open Shortest Path First)

Purpose:

- Determines the shortest network path

---

## BGP (Border Gateway Protocol)

Purpose:

- Exchanges routing information between large networks and ISPs

---

# ⭐ Important Concept
Protocol = Rules for Communication

Port = Door used by a Protocol

IP Address = Identity of Device

Example:
192.168.1.10 : 443

IP Address → Device  
Port 443 → HTTPS Service  
Protocol → HTTPS Rules
