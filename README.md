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
Key IOC: Lookalike domain with double "i" - accounts@premiiersugar.com

### 2. Ransomware (NetWalker Case Study)
A finance department workstation was compromised via a phishing email with a 
malicious invoice attachment. The malware established a C2 channel, encrypted 
files, and exfiltrated 48MB of data. The playbook covers host isolation, credential 
reset, backup validation, and recovery procedures.

**Key IOC:** winword.exe → powershell.exe → cmd.exe → vssadmin.exe execution chain

### 3. DDoS Attack
A multi-vector volumetric and application layer DDoS attack flooded the company's 
web portal with over 50Gbps of synthetic traffic. The playbook covers traffic 
profiling, cloud scrubbing centre diversion via BGP rerouting, WAF hardening, and 
service restoration.

**Key Metric:** Traffic must be rerouted to scrubbing centre within 12 minutes of 
trigger validation.

## Roles and Responsibilities
| Role | Responsibility |
|---|---|
| Incident Commander | Overall coordination and escalation decisions |
| SOC Analyst | Hands-on detection, analysis and threat hunting |
| Finance Lead | Financial assessment and payment freeze |
| IT Lead | Technical containment and system hardening |
| Legal & Compliance | Regulatory notification and evidence preservation |
| Communications Lead | Internal and external messaging |

## Key Metrics
| Metric | Target |
|---|---|
| MTTD (Mean Time to Detect) | Under 24 hours |
| MTTR (Mean Time to Respond) | Under 5 hours |
| Financial Recovery Window | Contact bank within 1 hour of discovery |
| DDoS Reroute Time | Within 12 minutes of trigger validation |

## Skills Demonstrated
- Incident response planning and documentation
- Threat actor TTPs analysis (BEC, Ransomware, DDoS)
- SIEM and EDR tool knowledge
- Communication strategy during active incidents
- MITRE ATT&CK framework alignment
- Metrics-driven security operations
