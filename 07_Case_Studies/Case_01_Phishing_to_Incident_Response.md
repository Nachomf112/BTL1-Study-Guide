# Case Study 01 – Phishing Email Leading to Security Incident

This case study simulates a **realistic SOC investigation workflow**, starting with a phishing email report and ending with incident response actions and documentation.

The objective is to demonstrate **end-to-end Blue Team analysis**, aligned with BTL1 and real SOC operations.

---

## 📌 Incident Summary

- **Incident Type:** Phishing leading to potential account compromise
- **Initial Detection Source:** User-reported email
- **SOC Role:** Tier 1 / Tier 2 Analyst
- **Status:** Confirmed security incident
- **Impact Level:** Medium

---

## ⏱️ Timeline Overview

| Time | Event |
|-----|------|
| 09:12 | User reports suspicious email |
| 09:18 | SOC begins phishing analysis |
| 09:32 | Malicious link confirmed |
| 09:45 | Suspicious login detected in SIEM |
| 10:05 | Incident escalated |
| 10:30 | Containment actions applied |

---

## 📧 Phase 1 – Phishing Analysis

### Observations

- Sender domain mimics a trusted service
- Urgent language requesting account verification
- Embedded URL redirects to an unknown domain

### Analysis Performed

- Header inspection revealed domain mismatch
- URL reputation check returned malicious classification
- Email content matches known credential harvesting patterns

### Conclusion

The email is confirmed as **malicious phishing**.

---

## 🧠 Phase 2 – Threat Intelligence Correlation

### Indicators Identified

- Malicious domain
- IP address associated with hosting infrastructure

### Threat Intelligence Findings

- Domain linked to recent phishing campaigns
- Infrastructure observed in multiple threat feeds
- No prior internal sightings

### MITRE ATT&CK Mapping

- **T1566.002 – Phishing: Link**
- **T1078 – Valid Accounts (potential risk)**

---

## 📊 Phase 3 – SIEM Investigation

### SIEM Findings

- Successful login to user account from unusual geolocation
- Login occurred shortly after phishing email interaction
- No prior history of logins from this region

### Correlation

- Phishing email timestamp aligns with suspicious authentication
- Indicates possible credential compromise

### Assessment

High confidence of **account compromise**.

---

## 🌐 Phase 4 – Network Analysis

### Network Indicators

- Outbound HTTPS connection to suspicious domain
- Short, periodic beacon-like traffic pattern
- Encrypted traffic prevents payload inspection

### Interpretation

Traffic characteristics consistent with **credential validation or session testing**.

---

## 🛡️ Phase 5 – Incident Response Actions

### Containment

- User account password reset
- Active sessions revoked
- Malicious domain blocked at gateway

### Eradication

- Email removed from all mailboxes
- IOC added to detection rules

### Recovery

- User access restored
- Increased monitoring enabled

---

## 📝 Phase 6 – Reporting and Documentation

### Incident Report Included

- Incident summary
- Timeline
- Evidence and IOCs
- Actions taken
- Final assessment

### Lessons Learned

- User awareness training recommended
- MFA enforcement prioritized
- Email filtering rules reviewed

---

## 📌 Final Assessment

This case demonstrates the importance of:

- User reporting
- Cross-module correlation (email, SIEM, network)
- Structured SOC workflows
- Clear documentation and communication

---

## 🔗 References and Standards

- MITRE ATT&CK – Phishing Techniques  
  https://attack.mitre.org/techniques/T1566/

- NIST SP 800-61 – Incident Handling Guide  
  https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final

- CISA – Phishing Guidance  
  https://www.cisa.gov/phishing

- Security Blue Team – BTL1 Overview  
  https://securityblue.team/blue-team-level-1/
