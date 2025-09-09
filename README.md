# 🚨 Cyber Security Internship – Task 2  
## Security Alert Monitoring & Incident Response (SOC Simulation)

![Splunk](https://img.shields.io/badge/Tool-Splunk-blue?logo=splunk&logoColor=white)  
![Security](https://img.shields.io/badge/Domain-Cyber%20Security-red?logo=hackaday&logoColor=white)  
![SOC](https://img.shields.io/badge/Focus-SOC%20Monitoring-orange?logo=linux&logoColor=white)  
![Internship](https://img.shields.io/badge/Internship-Future%20Intern-green?logo=github&logoColor=white)  

**Author:** Waggari Misganu Ebsa  
**Internship Submitted To:** Future Intern  
**Submission Date:** September 2025  
**Tools Used:** Splunk Cloud (Free Trial)  

---

## 📌 Executive Summary
This project simulated **Security Operations Center (SOC) activities** using **Splunk Cloud**, a Security Information and Event Management (SIEM) tool.  

The main objectives were:
- Detect suspicious activities such as brute-force login attempts and sensitive file access.  
- Classify incidents by severity (High, Medium).  
- Recommend remediation strategies to mitigate threats.  

🔍 **Key Findings:**  
- Multiple brute-force login attempts from suspicious IP addresses.  
- Unauthorized access to the `/etc/passwd` file (critical).  

---

## 📖 Introduction
### 🎯 Purpose
To simulate **real-world incident detection and response** by analyzing log data in Splunk Cloud.

### 📍 Scope
- **Log Source:** `sample_logs.txt` (simulated logs)  
- **Platform:** Splunk Cloud Free Trial  
- **Focus Areas:** Failed login attempts, brute-force indicators, sensitive file access events  

---

## ⚙️ Environment Setup & Exploration
- **Environment:** Splunk Cloud Free Trial  
- **Data:** Authentication attempts, usernames, IP addresses, and system access events  

### 🔎 Exploration Activities
- Verified ingestion of logs into Splunk  
- Executed SPL queries for failed logins, brute-force detection, and file access attempts  
- Correlated suspicious IP activity with system access events  

---

## 🚨 Incident Classification by Priority

| Incident Type             | IP Address   | Priority | Notes |
|----------------------------|-------------|----------|-------|
| Sensitive file access      | 192.168.1.10 | **High** | Unauthorized access to `/etc/passwd` |
| Brute-force login attempts | 192.168.1.11 | **High** | 3 failed login attempts |
| Brute-force login attempts | 192.168.1.12 | **High** | 3 failed login attempts |
| Repeated login failures    | 192.168.1.10 | **Medium** | 2 failed logins before success |

---

## 🛡️ Remediation & Recommendations

| Priority | Recommendation |
|----------|----------------|
| **High** | Enable account lockouts after multiple failed login attempts |
| **High** | Monitor and block suspicious IPs (e.g., 192.168.1.11, 192.168.1.12) |
| **High** | Enable alerts for sensitive file access such as `/etc/passwd` |
| **Medium** | Enforce strong password policies and monitor repeated login failures |
| **Medium** | Implement Multi-Factor Authentication (MFA) |

---

----
Special Thanks to Future Interns for this Attractive challenges
-----
Reach me @ wagarimisganu12@gmail.com
