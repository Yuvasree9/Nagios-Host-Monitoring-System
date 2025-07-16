# Nagios Host Monitoring System using Linux Guardian (CDAC Internship Project)

This project was developed during my cybersecurity internship at **CDAC, Noida** as part of the **Cyber Gyan Virtual Internship Program (August–September 2024)**. It focuses on building a host and service monitoring system using **Nagios Core** on **Kali Linux**, enhanced with **custom Linux Guardian scripts** for proactive network security and resource management.

## Problem Statement

In modern IT environments, the reliability, availability, and security of network infrastructure are critical. Manual monitoring becomes inefficient and prone to error as network complexity grows. This project aims to implement an automated, secure, and extensible monitoring solution using Nagios and Linux Guardian.

## Objectives

- Deploy Nagios Core to monitor both local and remote Linux hosts
- Extend monitoring capabilities with Linux Guardian custom scripts
- Automate alerting for system anomalies like failed SSH logins, high CPU usage, and service unavailability
- Secure communications and access through SSL/TLS, SSH, and firewalls

##  Technologies Used

- **Nagios Core** – Host & service monitoring
- **NRPE (Nagios Remote Plugin Executor)** – Remote monitoring agent
- **Kali Linux** – Monitoring environment
- **Linux Guardian System** – Custom security scripts
- **Apache Web Server** – Web interface for Nagios
- **SSL/TLS, SSH, Firewalls** – Secure access and communication

## System Architecture

- Central **Nagios Server** (on Kali Linux) monitors system health and services
- Remote Linux hosts are configured with **NRPE agents** for plugin execution
- **Nagios Plugins** and **custom Bash scripts** are used for resource monitoring and security checks
- Apache serves the Nagios web UI with admin authentication and IP restrictions

## Implementation Summary

1. **Nagios Setup on Kali Linux**
   - Installed and configured Nagios Core with web interface
   - Added Nagios plugins for essential checks

2. **Remote Host Configuration**
   - Installed and configured NRPE on remote machines
   - Set up commands to monitor CPU, memory, disk usage

3. **Linux Guardian Integration**
   - Created custom scripts to monitor failed SSH logins and other security events
   - Integrated scripts with Nagios for automated alerting

4. **Security Measures**
   - Enabled SSL/TLS for encrypted communication
   - Applied strong password policies, IP filtering, and Apache hardening

##  Potential Threats and Countermeasures

- **Unauthorized Access** → IP restriction, MFA, secure authentication
- **DoS/DDoS Attacks** → Firewall rules, rate limiting
- **Man-in-the-Middle** → SSL encryption, VPN tunnels
- **Plugin Exploits** → Input validation, strict permissions
- **Remote Code Execution** → AppArmor/SELinux policies and plugin audits

## Results

- Successfully implemented centralized monitoring of hosts and services
- Proactively detected critical resource usage and intrusion attempts
- Enabled real-time alerts via the Nagios dashboard and logs

## References

- [Nagios Core Docs](https://assets.nagios.com/downloads/nagioscore/docs/nagioscore/4/en/toc.html)
- [Nagios Plugins](https://www.nagios.org/projects/nagios-plugins/)
- [Kali Linux Docs](https://www.kali.org/docs/)
- [NRPE Manual (PDF)](https://assets.nagios.com/downloads/nagioscore/docs/nrpe/NRPE.pdf)
- [Nagios Video Tutorial](https://www.youtube.com/watch?v=lsL1nA8BJwA)

---

**Developed by:**  
**Thupalli Yuvasree**  
Project Trainee | CDAC Noida | Cybersecurity & Network Monitoring Intern (Aug–Sep 2024)
