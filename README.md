# BINCOM-ACADEMY-INTERNSHIP-4TH-CONTACT-ASSIGNMENT
Practical cybersecurity lab covering Elastic SIEM, NFS enumeration and hardening, NIST incident response, MITRE ATT&amp;CK, risk management, AI risk assessment, and prompt injection mitigation.
# BINCOM 4th Contact Assignment – Cybersecurity Assessment

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-blue)
![SIEM](https://img.shields.io/badge/SIEM-Elastic%20Stack-purple)
![Incident Response](https://img.shields.io/badge/Incident%20Response-NIST%20%7C%20MITRE%20ATT%26CK-orange)
![Risk Management](https://img.shields.io/badge/Risk%20Management-NIST%20RMF%20%7C%20ISO%2031000-green)
![AI Security](https://img.shields.io/badge/AI%20Security-Risk%20Assessment-red)
![Environment](https://img.shields.io/badge/Environment-Authorized%20Lab-lightgrey)

## Project Overview

This repository contains the documentation, configuration evidence, security analysis, and assessment outputs for my **BINCOM Academy 4th Contact Assignment**.

The project combines practical cybersecurity laboratory work with security governance and emerging AI-security concepts. The assessment covers:

- Security Information and Event Management (SIEM)
- Security monitoring and log collection
- Network service and NFS security assessment
- Incident response
- MITRE ATT&CK mapping
- NIST incident response methodology
- Risk management
- NIST Risk Management Framework (RMF)
- ISO 31000 risk management principles
- Securing AI agents
- AI risk assessment
- Prompt injection analysis and mitigation
- Integration of AI security considerations into incident response and monitoring

All practical activities were conducted within an **authorized cybersecurity laboratory environment** for educational and assessment purposes.

---

# 1. Assessment Objectives

The major objectives of this assignment were to demonstrate practical and theoretical understanding of:

1. Deploying and validating a functional SIEM environment.
2. Collecting and analyzing system security logs.
3. Investigating an exposed network service.
4. Identifying security risks associated with NFS configuration.
5. Applying a controlled remediation to reduce the identified risk.
6. Documenting an incident response process.
7. Mapping observed activities to MITRE ATT&CK techniques.
8. Applying risk management principles using NIST RMF and ISO 31000 concepts.
9. Assessing security risks associated with AI agents and generative AI systems.
10. Understanding prompt injection attacks and appropriate defensive controls.
11. Integrating AI-related risks into incident response and security monitoring.

---

# 2. Laboratory Environment

The practical assessment was performed using an isolated VirtualBox laboratory.

### Security Workstation

**Kali Linux**

- Host-Only IP: `192.168.56.101`
- NAT interface: `10.0.2.15`
- Primary role:
  - Security testing
  - Network enumeration
  - NFS investigation
  - SIEM administration
  - Log analysis

### Target System

**Metasploitable2**

- Host-Only IP: `192.168.56.103`
- Primary role:
  - Deliberately vulnerable laboratory target
  - NFS security investigation
  - Network service enumeration

### Network

```text
                    VirtualBox NAT
                         |
                    10.0.2.0/24
                         |
                  +--------------+
                  | Kali Linux   |
                  | 10.0.2.15    |
                  | 192.168.56.101
                  +--------------+
                         |
                    Host-Only LAN
                    192.168.56.0/24
                         |
                  +--------------+
                  | Metasploitable2 |
                  | 192.168.56.103  |
                  +--------------+
