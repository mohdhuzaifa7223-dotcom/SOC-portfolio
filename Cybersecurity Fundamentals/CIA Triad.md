# CIA Triad - Cybersecurity Fundamentals

## What is the CIA Triad?

The **CIA Triad** is one of the most important security models in cybersecurity. It consists of three core principles that help protect information and systems.

* **C** – Confidentiality
* **I** – Integrity
* **A** – Availability

---

# 1. Confidentiality

### Definition

Confidentiality ensures that **only authorized users can access sensitive information**.

### Goal

Prevent unauthorized access to data.

### Examples

* Strong Passwords
* Multi-Factor Authentication (MFA)
* Encryption
* Access Control (RBAC)
* File Permissions

### Real-Life Example

Only the HR department can view employees' salary information.

### Threats

* Data Breaches
* Phishing
* Password Theft
* Insider Attacks

---

# 2. Integrity

### Definition

Integrity ensures that **data remains accurate and is not modified without authorization**.

### Goal

Protect data from unauthorized changes.

### Examples

* Hashing
* Digital Signatures
* Checksums
* Version Control
* File Integrity Monitoring

### What is Hashing?

Hashing is a **one-way process** that converts data into a fixed-length value called a **hash**.

Example:

Original Password:

```text
MyPassword123
```

Hash:

```text
8f434346648f6b96...
```

If even **one character changes**, the hash changes completely.

### Password Verification Process

```text
User enters password
        │
        ▼
Server hashes the password
        │
        ▼
Compare with stored hash
        │
        ├── Match → Login Successful ✅
        └── No Match → Login Failed ❌
```

### Where Hashing is Used

* Password Storage
* File Integrity Verification
* Digital Signatures
* Malware Detection
* SOC File Integrity Monitoring

### Threats

* Malware
* Unauthorized File Changes
* SQL Injection
* Data Tampering

---

# 3. Availability

### Definition

Availability ensures that **authorized users can access systems and data whenever they need them**.

### Goal

Keep systems running without interruption.

### Examples

* Backups
* Redundant Servers
* Failover Systems
* Disaster Recovery
* Load Balancers
* UPS (Uninterruptible Power Supply)

### Real-Life Example

An e-commerce website remains online during a festival sale because it uses redundant servers and load balancing.

### Threats

* DDoS Attacks
* Hardware Failure
* Power Outages
* Ransomware
* Natural Disasters

---

# CIA Triad Summary

| Principle       | Goal                         | Protection Methods                               |
| --------------- | ---------------------------- | ------------------------------------------------ |
| Confidentiality | Prevent unauthorized access  | Encryption, MFA, Passwords, Access Control       |
| Integrity       | Prevent unauthorized changes | Hashing, Digital Signatures, Checksums           |
| Availability    | Keep systems accessible      | Backups, Redundancy, Failover, Disaster Recovery |

---

# Encryption vs Hashing

| Encryption                            | Hashing                                     |
| ------------------------------------- | ------------------------------------------- |
| Protects Confidentiality              | Protects Integrity                          |
| Two-way process                       | One-way process                             |
| Can be decrypted with the correct key | Cannot be reversed                          |
| Used to keep data secret              | Used to verify data integrity and passwords |

---

# Why the CIA Triad Matters in SOC

SOC (Security Operations Center) analysts use the CIA Triad to understand and respond to security incidents.

Examples:

* Customer data stolen → **Confidentiality**
* Database records modified → **Integrity**
* Website unavailable due to DDoS → **Availability**

---

# Key Takeaways

* **Confidentiality** → Keep data secret.
* **Integrity** → Ensure data is accurate and unchanged.
* **Availability** → Keep systems and data accessible.
* **Encryption** protects confidentiality.
* **Hashing** protects integrity.
* The **CIA Triad** is the foundation of cybersecurity and is essential knowledge for every SOC analyst.

