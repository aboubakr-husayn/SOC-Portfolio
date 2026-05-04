# SIEM-Based Brute Force Attack Detection Using Splunk

## Project Overview

This project focuses on implementing a SIEM-based detection system using Splunk to identify potential brute-force attacks on a Windows environment.

The project involves analyzing Windows Security Event Logs to detect suspicious authentication behavior, particularly repeated failed login attempts that may indicate unauthorized access attempts.

---

## Objectives

- Monitor Windows authentication activity using SIEM
- Detect brute-force attack patterns
- Correlate failed and successful login events
- Build a SOC-style monitoring dashboard
- Configure alerts for real-time detection

---

## Tools & Technologies

- Splunk Enterprise (SIEM)
- Windows Security Event Logs
- Log Analysis & Correlation
- Splunk Dashboards
- Alerting System

---

## Key Event IDs

- **Event ID 4625** – Failed login attempt  
- **Event ID 4624** – Successful login  

---

## Implementation Details

- Ingested Windows Security Logs into Splunk
- Analyzed failed login attempts using Event ID 4625
- Aggregated login failures by account and host
- Correlated failed (4625) and successful (4624) login events
- Identified accounts with suspicious login patterns
- Visualized login activity using dashboards
- Monitored login attempts over time to detect spikes
- Identified potential compromised accounts
- Analyzed source hosts and IP addresses of login attempts
- Configured threshold-based alerting (failed attempts > 5)

---

## Detection Logic

The detection mechanism is based on:

- High number of failed login attempts within a short time period
- Multiple failed attempts targeting specific accounts
- Failed login attempts followed by a successful login

These patterns may indicate brute-force attacks or compromised user accounts.

---

## SOC Analysis Insights

- Accounts with repeated failed logins are high-risk targets
- Sudden spikes in login failures indicate possible attack activity
- Correlation between failed and successful logins may indicate compromise
- Source IP analysis helps identify attack origin (internal vs external)

---

## SOC Skills Demonstrated

- SIEM monitoring and log analysis  
- Event correlation and threat detection  
- Brute-force attack detection  
- Windows Event Log investigation  
- Dashboard creation and visualization  
- Alert configuration and tuning  
- Security monitoring workflow (SOC operations)  

---

## Full Project Report

📄 [Download Full Report](./SIEM-Based-Brute-Force-Detection-Using-Splunk.docx)

---

## Conclusion

This project demonstrates practical SOC-level skills in detecting brute-force attacks using Splunk. It highlights the importance of log analysis, event correlation, and real-time alerting in identifying and responding to security threats.

The implementation reflects real-world SOC workflows used to monitor, detect, and respond to authentication-based attacks.
