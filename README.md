# Web Application Security Audit & Hardening
## OWASP Top 10 Laboratory Series

This repository contains a series of technical labs focused on identifying, exploiting, and mitigating vulnerabilities in a web application (HuskyHub). These labs demonstrate proficiency in the **OWASP Top 10** framework, moving from initial reconnaissance to advanced cryptographic implementation.

### 🛠 Technologies & Tools
* **Security & Recon:** Wireshark, Burp Suite, Chrome DevTools, Nmap
* **Development & DevOps:** Docker Desktop, Docker Compose, Python (Flask), Nginx
* **Cryptography & Auth:** OpenSSL, Bcrypt, JWT/Session Management
* **Database:** MySQL / MariaDB

---

### 📂 Lab Directory

#### [Lab 1: Reconnaissance & Attack Surface Mapping](./lab-01-recon.md)
* **Focus:** Information Exposure and Identification of Attack Vectors.
* **Key Actions:** Conducted structured reconnaissance using Browser DevTools to inspect HTTP response headers and cookies. Analyzed page source code for leaked internal paths, developer comments, and insecure hidden form fields. 
* **AI Security:** Performed initial prompt injection testing on an integrated AI Academic Advisor to identify data privacy risks.

#### [Lab 2: Networking, Packet Capture, and MitM](./lab-02-mitm.md)
* **Focus:** Broken Access Control and Identification/Authentication Failures.
* **Key Actions:** Conducted ARP spoofing to intercept unencrypted HTTP traffic. Utilized Wireshark to capture session cookies and performed session hijacking through manual token replacement in the browser.
* **Key Learning:** Analyzing the critical distinction between authentication (proving identity) and session management (maintaining identity).

#### [Lab 3: Cryptography & Secure Communication](./lab-03-crypto.md)
* **Focus:** Cryptographic Failures and Security Misconfiguration.
* **Key Actions:** Migrated a plaintext user database to a hashed format using **bcrypt** with randomized salts. Configured an **Nginx** reverse proxy to enforce **HTTPS/TLS** encryption using OpenSSL-generated certificates.
* **Key Learning:** Implementing "Defense in Depth" by securing sensitive data both at rest and in transit.

---

### 🧠 Core Competencies
* **Vulnerability Assessment:** Identifying insecure protocols, unencrypted data flows, and information leaks.
* **Secure Development:** Implementing industry-standard hashing algorithms and secure header configurations.
* **Network Security:** Configuring secure communication channels and understanding local network broadcast risks.
* **The Adversarial Mindset:** Thinking like a "Committed Attacker" to anticipate exploits before they occur.

---
*Note: These labs were conducted in a controlled environment for educational purposes as part of a Cybersecurity curriculum.*
