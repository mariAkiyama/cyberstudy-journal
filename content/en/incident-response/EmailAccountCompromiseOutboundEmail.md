---
title: "Email Account Compromise and Malicious Outbound Mail"
draft: false
bookCollapseSection: true
weight: 10
---
## Incident Response in Action: Email Account Compromise and Malicious Outbound Mail

### Scenario
An employee’s email account was compromised, and suspicious emails were sent to both internal and external recipients. 
The incident was discovered after a business partner reported receiving a suspicious message.


---

## 1. Immediate User Actions (CSIRT Instructions)

* **Reset the compromised account password** immediately. Ensure it is strong and unique.
* **Review mailbox rules and forwarding**: remove any unauthorized rules or auto-forwarding.

---

## 2. Technical Containment

**Technical Team:**

* Invalidate all active sessions (cloud, email, VPN).
* Revoke VPN sessions and block suspicious IPs.
* Preserve logs (email, VPN, endpoint, proxy).

---

## 3. Forensic Investigation

**Forensic Team:**

* Analyze suspicious logins (IP, device, region, timing).
* Examine endpoint(s) for malware, persistence mechanisms, or lateral movement.
* Review mailbox and file access logs.
* Check email forwarding rules, OAuth app authorizations, and any suspicious scripts.
* Preserve chain of evidence for potential legal or regulatory proceedings.
* Coordinate with Legal/Compliance if sensitive data exposure is suspected.

---

## 4. Legal & Compliance

**Legal/Compliance Team:**

* Determine if sensitive or regulated data was exposed.
* Check contractual obligations and reporting requirements.
* Advise CSIRT on regulatory notifications and escalation procedures.

---

## 5. Communications & External Coordination

**PR/Communications Team:**

* Prepare notifications to affected recipients (warning not to open/click suspicious emails).
* Coordinate messages with Legal and Management.
* Prepare potential media statements if incident escalates.

**Management Liaison:**

* Brief executives on business impact and reputational risk.

---

## 6. Recovery & Remediation

**Technical Team:**

* Clean or reimage compromised endpoints.
* Restore secure account access (MFA enforced).
* Update monitoring rules and tighten email security policies.

---

## 7. Lessons Learned & Governance

**CSIRT & All Teams:**

* Conduct post-incident review: document root cause, actions, and lessons learned.
* Strengthen policies: mandatory MFA, password policies, log retention.
* Educate users on phishing, reporting suspicious activity, and safe email practices.

---

