# 🛡️ Security Concept

# 🔑 Authentication, Credentials, and Authorization

## Authentication

Authentication is the process of verifying the identity of a user, device, or system.

It answers:

**"Who are you?"**

Examples:

- Username and password
- Fingerprint
- Face recognition
- Multi-Factor Authentication (MFA)

---

## Credentials

Credentials are information used to prove identity.

Examples:

- Username
- Password
- Security tokens
- Digital certificates

---

## Authorization

Authorization determines what resources or actions an authenticated user is allowed to access.

It answers:

**"What are you allowed to do?"**

Example:

- Normal user → Can view files
- Administrator → Can modify system settings

---

# 🔐 Cryptography

Cryptography is the practice of protecting information by converting readable data into a secure format.

Main purposes:

- Protect confidentiality
- Maintain data integrity
- Secure communication

---

# 🔒 Encryption

Encryption converts readable information (**Plaintext**) into unreadable information (**Ciphertext**).

Purpose:

- Prevent unauthorized access
- Protect sensitive data

Example:

Banking information is encrypted during online transactions.

---

# 🔓 Decryption

Decryption converts encrypted data (**Ciphertext**) back into its original readable form (**Plaintext**).

It requires the correct key to access the information.

---

# 🔥 Firewall

A firewall is a security system that acts like a **security guard** between trusted and untrusted networks.

It monitors and controls network traffic based on security rules.

---

# Firewall Functions

## Incoming Traffic Monitoring

Checks traffic coming into a network.

Examples:

- Blocking suspicious connections
- Allowing trusted requests

---

## Outgoing Traffic Monitoring

Checks traffic leaving a network.

Examples:

- Preventing unauthorized data transfer
- Detecting suspicious communication

---

## Blocking Unauthorized Access

Firewall can:

- Block malicious connections
- Restrict unwanted traffic
- Protect systems from network attacks

---

# Types of Firewall

## Network Firewall

Protects entire networks.

Example:

Company network firewall.

---

## Host Firewall

Installed on individual devices.

Example:

Computer firewall.

---

## Application Firewall

Protects specific applications and web services.

Example:

Web Application Firewall (WAF).

---

# Firewall Rule Example

Allow:

- Trusted IP addresses
- Required services

Block:

- Unknown connections
- Suspicious traffic

---

# 🛡️ Security Protection Flow

User Authentication  
⬇️  
Authorization Check  
⬇️  
Firewall Filtering  
⬇️  
Encrypted Communication  
⬇️  
Secure Data Access

---

# 🧱 Defense in Depth

Defense in Depth is a security strategy that uses multiple layers of security controls.

Purpose:

- Prevent attacks
- Reduce impact of successful attacks
- Provide multiple security barriers

Examples:

- Firewall
- Antivirus
- Encryption
- Access control
- Monitoring systems
- Backups

Example:

If an attacker bypasses the firewall, another security layer like authentication can stop them.

---

# 🚫 Least Privilege Principle

Least Privilege means users should receive only the minimum access required to perform their tasks.

Benefits:

- Reduces unauthorized access
- Limits damage from compromised accounts

Example:

An employee does not need administrator access for normal work.

---

# 🏰 Zero Trust Security

Zero Trust follows the principle:

**"Never Trust, Always Verify"**

Every user, device, and connection must be verified before access is granted.

Key principles:

- Verify identity
- Verify device security
- Limit access
- Monitor continuously

---

# 🔐 Access Control

Access control manages who can access resources and what actions they can perform.

Types:

## Mandatory Access Control (MAC)

Strict access rules controlled by the system.

## Discretionary Access Control (DAC)

Resource owners decide permissions.

## Role-Based Access Control (RBAC)

Access based on user roles.

Example:

- Admin
- Manager
- Employee

---

# 🧾 Security Policies

Security policies define rules and procedures for protecting an organization.

Examples:

- Password policy
- Acceptable use policy
- Data protection policy
- Incident response policy

---

# 🔑 Multi-Factor Authentication (MFA)

MFA requires multiple verification methods before granting access.

Authentication factors:

## Something You Know

- Password
- PIN

## Something You Have

- Mobile device
- Security token

## Something You Are

- Fingerprint
- Face recognition

Benefits:

- Prevents account takeover
- Protects stolen passwords

---

# 🔄 Patch Management

Patch management is the process of identifying, testing, and applying software updates.

Purpose:

- Fix vulnerabilities
- Improve security
- Improve stability

Steps:

1. Identify missing patches
2. Test updates
3. Deploy patches
4. Verify installation

---

# 📊 Security Monitoring

Security monitoring continuously observes systems for suspicious activities.

Monitors:

- Network traffic
- User activities
- System logs
- Applications

Tools:

- SIEM
- IDS
- IPS

---

# 📁 Logging

Logs are records of system activities.

Examples:

- Login attempts
- Network connections
- Application events

Logs help with:

- Investigation
- Threat detection
- Digital forensics

---

# 🖥️ SIEM (Security Information and Event Management)

SIEM collects and analyzes security logs from different sources.

Functions:

- Log collection
- Threat detection
- Alert generation
- Security investigation

Examples:

- Splunk
- IBM QRadar
- Microsoft Sentinel

---

# 🚨 Security Alert

A security alert is a notification generated when suspicious activity is detected.

Examples:

- Multiple failed login attempts
- Malware detection
- Unusual network traffic

---

# 🕵️ Threat Intelligence

Threat intelligence is information about current and potential cyber threats.

Used for:

- Understanding attackers
- Detecting threats
- Improving defenses

Sources:

- Security researchers
- Threat databases
- Security reports

---

# 🔎 Threat Hunting

Threat hunting is the proactive search for hidden threats inside systems.

Unlike normal detection, threat hunting actively searches for attackers.

Activities:

- Analyze logs
- Search suspicious behavior
- Investigate unusual activities

---

# 🧪 Vulnerability Management

A continuous process of finding and fixing security weaknesses.

Lifecycle:

1. Discover assets
2. Scan vulnerabilities
3. Analyze risk
4. Fix vulnerabilities
5. Verify improvements

---

# 📝 Security Assessment

Security assessment evaluates the effectiveness of security controls.

Includes:

- Vulnerability assessment
- Penetration testing
- Security audits

---

# 🛡️ Endpoint Security

Endpoint security protects devices connected to a network.

Examples:

- Computers
- Laptops
- Mobile devices
- Servers

Protection:

- Antivirus
- Endpoint Detection and Response (EDR)
- Device control

---

# 🌐 Network Security

Network security protects communication and infrastructure.

Includes:

- Firewalls
- IDS/IPS
- VPN
- Network segmentation

---

# 🔒 Data Security

Protecting information from unauthorized access, modification, or destruction.

Methods:

- Encryption
- Access control
- Backup
- Data Loss Prevention (DLP)

---

# 💾 Backup and Disaster Recovery

Backup creates copies of important data.

Types:

- Full backup
- Incremental backup
- Differential backup

Disaster Recovery ensures systems can return to normal after incidents.

---

# 📱 Security Awareness

Security awareness trains users to recognize and prevent cyber threats.

Topics:

- Phishing awareness
- Password security
- Safe browsing
- Data protection

---

# 🧬 Digital Signature

A digital signature verifies:

- Authenticity
- Integrity
- Non-repudiation

Uses:

- Software verification
- Secure documents

---

# 📜 Digital Certificate

A digital certificate proves the identity of a website, user, or organization.

Used in:

- HTTPS
- Secure communication

---

# 🌍 HTTPS

HTTPS is the secure version of HTTP.

Provides:

- Encryption
- Authentication
- Data integrity

Uses:

- TLS/SSL certificates

---

# 🔄 Incident Response

Incident response is the process of handling cybersecurity incidents.

Steps:

1. Preparation
2. Detection
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

---

# 🧠 Security Mindset

A cybersecurity professional should:

- Think like an attacker
- Understand defenses
- Continuously learn
- Follow ethical practices
- Protect information assets
