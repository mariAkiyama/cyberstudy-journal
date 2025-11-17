---
title: "Cybersecurity Technology Stack - Example"
draft: false
bookCollapseSection: true
weight: 10
---
## Cybersecurity Technology Stack

### An example of security stack
A Cybersecurity Technology Stack is the layered collection of integrated tools and solutions an organization deploys to achieve defense-in-depth across its infrastructure.
The map below provides an example of such a stack, detailing common tools and how their capabilities are mapped directly to defensive measures **MITRE D3FEND tactics** to counter known adversary behaviors **MITRE ATT&CK**.

---

| Security Stack Layer | Priority | Popular Tools | D3FEND Tactic | D3FEND Technique | Attack Phase | Description / Core Function 					| 
| :---	 | :---		 | :---		 | :---		 | :---		 | :---		 | :---		 |
|**Vulnerability Management**	 | 	High	 | 	Microsoft Defender Vulnerability Management, Tenable, Qualys, Rapid7, Nessus	 | 	Model / Harden	 | 	Network Vulnerability Assessment, Software Update	 | 	Reconnaissance & Weaponization	 | 	Continuous process of identifying, prioritizing, and remediating weaknesses (missing patches, misconfigurations) in software and hardware to reduce the attack surface.	
|**Security Awareness Training**	 | 	High	 | 	Microsoft Defender for Office 365 Attack Simulation, KnowBe4, PhishMe, Cofense, Proofpoint	 | 	Harden	 | 	User Behavior Baseline	 | 	Targeting	 | 	Addresses the human factor by educating employees on social engineering, phishing, and proper handling of sensitive data.	
|**Cloud Security Posture Management (CSPM)**	 | 		 | 	Microsoft Defender for Cloud, Wiz, Orca Security, Cloud Security Hubs (AWS/Azure/GCP)	 | 	Harden / Model	 | 	Platform Hardening, Access Modeling	 | 	Configuration	 | 	Monitors and enforces security policies across cloud environments (IaaS/PaaS) to prevent critical misconfigurations (e.g., open storage buckets, overly permissive IAM roles).	
|**Application Security (AppSec)**	 | 		 | 	Microsoft Defender for DevOps,Azure DevOps/GitHub Security, Checkmarx, SonarQube (SAST/DAST), Snyk (SBOM)	 | 	Harden	 | 	Input Validation	 | 	Design	 | 	Embeds security into the development lifecycle (DevSecOps) to find and fix vulnerabilities in custom application code before deployment.	
|**Network Security (Firewall/IDS/IPS)**	 | 		 | 	Palo Alto Networks, Cisco, Fortinet(FortiGate), Juniper, Check Point Quantum	 | 	Harden / Detect	 | 	Network Traffic Filtering, Network Protocol Analysis	 | 	Initial Access	 | 	Controls and monitors traffic at network boundaries and internal segments, blocking known threats and analyzing protocol behavior for anomalies.	
|**Identity & Access Management (IAM)**	 | 		 | 	Microsoft Entra ID, Okta, Ping Identity, AWS IAM, Google Cloud Identity	 | 	Harden	 | 	Account Disabling, Role-Based Access Control	 | 	Initial Access	 | 	Manages and secures user identities, governing who can access which resources, managing entitlements, and enforcing provisioning/de-provisioning processes.	
|**IAM - Multi-Factor Authentication (MFA)	 | 	High	 | 	Microsoft Authenticator, Duo, BeyondTrust, YubiKey	 | 	Harden	 | 	Multi-Factor Authentication	 | 	Initial Access	 | 	Adds a required second layer of verification beyond the password, drastically reducing the risk of unauthorized access from stolen or brute-forced credentials.	
|**End-User Protection (EDR/Antivirus)**	 | 	High	 | Microsoft Defender,	CrowdStrike Falcon, SentinelOne, Palo Alto Networks Cortex XDR,  Sophos Intercept X	 | 	Detect / Isolate	 | 	Malware Analysis, Process Monitoring, Host Isolation	 | 	Execution, Lateral Movement	 | 	Secures endpoints (laptops, servers) by continuously monitoring activity, detecting malicious behavior (not just signatures), and isolating compromised hosts.	
|**Privileged Access Management (PAM)**	 | 		 | 	Microsoft Entra ID Privileged Identity Management (PIM), CyberArk, Delinea, HashiCorp Vault, BeyondTrust	 | 	Harden / Evict	 | 	Credential Hardening, Credential Revoking	 | 	Privilege Escalation	 | 	Secures, manages, and monitors accounts with elevated permissions (admin, root), enforcing least privilege and isolating privileged sessions to prevent credential theft.	
|**Network Segmentation (NAC)**	 | 		 | 	Cisco ISE, Aruba ClearPass, Illumio	 | 	Isolate	 | 	Network Segmentation	 | 	Lateral Movement	 | 	Divides the network into isolated zones to restrict the blast radius of an attack, ensuring an intruder on one segment cannot freely move to others.	
|**Security Information & Event Management (SIEM)**	 | 		 | 	Microsoft Sentinel, Splunk, IBM QRadar, Elastic Security	 | 	Detect	 | 	Log Analysis, Identifier Activity Analysis	 | 	C2 & Detection	 | 	The central security brain. Aggregates, normalizes, and correlates security logs from every tool and system to detect complex, multi-stage attacks in real-time.	
|**Threat Intelligence (TI)**	 | 		 | 	Microsoft Defender Threat Intelligence, Recorded Future, Mandiant, Commercial TI Feeds	 | 	Detect	 | 	Indicator Analysis	 | 	C2 & Detection	 | 	Provides external context on current and emerging threats, IoCs (IPs, hashes), and adversary TTPs, enriching SIEM alerts and improving detection rules.	
|**Data Loss Prevention (DLP)**	 | 		 | 	Microsoft Purview, Symantec, Forcepoint, Trellix DLP	 | 	Isolate	 | 	Data Loss Restriction	 | 	Exfiltration	 | 	Identifies, monitors, and protects sensitive data (PII, IP, financial data) in motion, at rest, or in use, blocking unauthorized data from leaving the organization.	
|**SOAR**	 | 		 | 	Microsoft Sentinel Automation & Orchestration. Splunk Phantom, Cortex XSOAR, Swimlane, Torq	 | 	Evict / Restore	 | 	Automated Response	 | 	Containment & Response	 | 	Automates and orchestrates security workflows (playbooks), connecting and instructing tools across the stack (e.g., taking an SIEM alert and automatically blocking an IP on the firewall).	
|**Incident Response (IR) / DR**	 | 		 | 	Veeam (Backup), Rubrik,  Cohesity	 | 	Restore	 | 	File Restoration	 | 	Impact & Recovery	 | 	Defines the plans and uses the tools for containing, eradicating, and recovering from a major security breach or disaster (e.g., restoring clean data from backups).	

---

