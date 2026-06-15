# 🛡️ Security Concepts
---

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
