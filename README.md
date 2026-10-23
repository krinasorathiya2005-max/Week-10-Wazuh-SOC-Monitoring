# 🛡️ Week 10: SOC – Wazuh SIEM Setup & Alert Monitoring

![Cybersecurity](https://img.shields.io/badge/Domain-Cybersecurity-blue)
![SIEM](https://img.shields.io/badge/Platform-Wazuh-orange)
![Monitoring](https://img.shields.io/badge/Focus-Security%20Monitoring-green)
![Project](https://img.shields.io/badge/Type-Hands--On%20Lab-success)

## 📌 Project Overview

This project focuses on practical Security Operations Center (SOC) workflows using Wazuh, an open-source security monitoring platform.

The objective is to understand endpoint monitoring, security event collection, alert investigation, incident classification, and response recommendations in an authorized cybersecurity laboratory.

The project also explores how Wazuh and Snort IDS can provide complementary endpoint and network security visibility.

## 🎯 Project Objectives

- Understand Wazuh SIEM fundamentals and architecture.
- Configure and verify the Wazuh monitoring environment.
- Monitor endpoints using the Wazuh Agent.
- Investigate authentication and file integrity events.
- Analyze security alerts using timestamps, rule IDs, severity, and event details.
- Document a high-interest security alert.
- Understand incident containment, recovery, and lessons learned.
- Explore the relationship between Wazuh SIEM and Snort IDS.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| Wazuh | Security monitoring and alert investigation |
| Wazuh Agent | Endpoint telemetry collection |
| Wazuh Manager | Event processing and rule analysis |
| Wazuh Dashboard | Security event visualization and investigation |
| Snort IDS | Network intrusion detection |
| Windows/Linux VMs | Authorized laboratory environment |
| GitHub | Project documentation and version control |

## 🏗️ Monitoring Architecture

```text
Monitored Endpoint
       |
       v
  Wazuh Agent
       |
       v
  Wazuh Manager
       |
       v
 Rule Analysis
       |
       v
 Wazuh Dashboard
       |
       v
   SOC Analyst
       |
       v
Investigation and Response
```

## 🔍 Investigation Workflow

1. Prepare and verify the Wazuh environment.
2. Install and register a monitored endpoint.
3. Confirm agent connectivity.
4. Generate controlled security events in the lab.
5. Review alerts in the Wazuh Dashboard.
6. Investigate timestamps, agent details, rule IDs, severity, and event context.
7. Identify related activity and assess potential impact.
8. Document findings and recommend appropriate response actions.

## 🚨 High-Interest Alert Case Study

The report includes an example involving a Snort alert:

**Detection:** ET SCAN Nmap Scripting Engine User-Agent Detected

**Rule ID:** 2100498  
**Reported severity:** Level 4 — Medium  
**Source IP:** 192.168.56.1  
**Destination IP:** 192.168.56.11  
**Destination port:** 80/TCP

The alert indicates possible network reconnaissance. The analyst should verify whether the activity was authorized, review supporting evidence, and investigate related events before determining whether an incident occurred.

An alert alone does not prove a successful compromise.

## 📂 Repository Structure

```text
Week-10-Wazuh-SOC-Monitoring/
├── README.md
├── docs/
│   └── Week_10_Wazuh_SOC_Report.docx
├── screenshots/
│   ├── wazuh-dashboard.png
│   ├── wazuh-agent.png
│   ├── security-alerts.png
│   └── incident-investigation.png
└── presentation/
    └── Week_10_Presentation.pptx
```

*This is a suggested structure. Update the filenames to match the files actually uploaded.*

## 📚 Key Learning Outcomes

- Understanding SIEM-based security monitoring.
- Learning how endpoint agents communicate with a monitoring server.
- Investigating security alerts using evidence and context.
- Understanding false positives and alert prioritization.
- Applying incident response concepts.
- Learning why endpoint and network telemetry can complement each other.

## 🔐 Ethical Disclaimer

This project is intended for educational purposes and authorized security testing only. All monitoring and testing must be performed on systems for which permission has been granted.

## 👨‍💻 Author

**Krina Sorathiya**  
Cybersecurity Learner | SOC Analyst Aspirant



---

⭐ If you find this project useful, consider starring the repository.
