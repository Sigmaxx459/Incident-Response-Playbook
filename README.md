# Incident-Response-Playbook
##Overview
A structured incident response developed for Golden Crunch Biscuits Ltd, a fictional manufacturing company. The playbook provides step-by-step response procedures for three real-world scenarios: Business Email Compromise (BEC), Ransomware and Distributed Denial of Service(DDOS). It covers the full incident response lifecycle and is designed for use by Security Operations, Finance, Legal and Executive teams.

##Objectives
Develop a structured IR framework covering detection through post-incident review
Define clear roles and responsibilities for each team during an incident
Establish communication strategies for internal and external stakeholders
Document containment, eradication and recovery procedures for each attack type
Define success metrics including MTTD and MTTR targets

##Tools Technologies Referenced
Tool & Purpose
Splunk / Microsoft Sentinel | SIEM - log correlation and alerting
CrowdStrike Falcon / Microsoft Defender | EDR - endpoint threat detection
Mimecast / Defender for office 365 | Email security gateway
Palo Alto NGFW /Cisco ASA | Firewall and traffic filtering
VirusTotal / MISP | Threat intelligence
Snort / Suricata | IDS/IPS - network intrusion detection
## Scenarios Covered
### 1. Business Email Compromise
A threat actor impersonated a trusted supplier (Premier Sugar Refineries) using a lookalike domain (accounts@premiiersugar.com) to redirect a payment. The playbook covers email header analysis, financial containment, supplier verification and eradication procedures.
Key IOC: Lookalike domain with double "i" - accounts@premiiersugar.comIncident response playbook covering BEC, Ransomware and DDos attacks scenarios including detection, containment, eradication and recovery procedures.
