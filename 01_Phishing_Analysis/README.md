# Phishing Analysis

Phishing remains one of the **most common initial access vectors** used by attackers. As a result, phishing analysis is a **core responsibility of Security Operations Center (SOC) analysts**, especially at junior and entry levels.

This module focuses on the **systematic analysis of phishing emails**, combining technical inspection with contextual and behavioral analysis.

---

## 🎯 Objectives of Phishing Analysis

The primary goals when analyzing a phishing email are:

- Determine whether the email is malicious or benign
- Identify indicators of compromise (IOCs)
- Assess potential impact and risk
- Provide clear conclusions and recommendations
- Support containment and remediation actions

Phishing analysis is not only about detecting malicious intent, but also about **communicating findings clearly and accurately**.

---

## 🧠 Analyst Mindset

Effective phishing analysis requires a **methodical and skeptical mindset**:

- Do not assume malicious intent without evidence
- Correlate multiple indicators before reaching conclusions
- Focus on what is abnormal for the organization or user
- Prioritize clarity and evidence over speculation

SOC analysts must balance **speed and accuracy**, especially when handling high email volumes.

---

## 📧 Key Elements to Analyze in a Phishing Email

### 1️⃣ Sender Information
- Display name vs. actual email address
- Domain reputation and age
- Lookalike or typo-squatted domains

### 2️⃣ Email Headers
- `From`, `Return-Path`, and `Reply-To` mismatches
- SPF, DKIM, and DMARC results
- Mail relay path anomalies

### 3️⃣ Email Content
- Urgency or pressure tactics
- Generic greetings
- Requests for credentials, payments, or sensitive data
- Grammar, spelling, or formatting inconsistencies

### 4️⃣ URLs and Links
- Mismatch between visible and actual URLs
- Use of URL shorteners
- Suspicious domains or IP-based links

### 5️⃣ Attachments
- Unexpected attachments
- Executable or macro-enabled file types
- Archive files containing scripts or binaries

---

## 🔍 Common Phishing Techniques

- Credential harvesting pages
- Business Email Compromise (BEC)
- Invoice and payment fraud
- Account suspension or password reset lures
- Malware delivery via attachments or links

Understanding these patterns helps analysts quickly identify **high-risk emails**.

---

## 🛠️ Tools Commonly Used in Phishing Analysis

While tools may vary between organizations, common categories include:

- Email header analyzers
- URL reputation and sandbox services
- Attachment analysis tools
- Threat intelligence platforms
- SIEM and email security gateways

The emphasis should always be on **interpreting results**, not just collecting them.

---

## 📝 Documentation and Reporting

A phishing analysis report should include:

- Summary of findings
- Evidence supporting the conclusion
- Identified IOCs
- Recommended actions (block, quarantine, user awareness, etc.)

Clear documentation ensures findings can be acted upon by other teams.

---

## 📌 Key Takeaway

Phishing analysis is a **foundational SOC skill** that combines:

- Technical inspection
- Behavioral analysis
- Risk assessment
- Clear communication

Mastering this process is essential for effective Blue Team operations.

---

## 🔗 Official and Trusted References

- CISA – Avoiding Social Engineering and Phishing Attacks:  
  https://www.cisa.gov/avoid-social-engineering-and-phishing-attacks

- NIST SP 800-177 – Trustworthy Email:  
  https://csrc.nist.gov/publications/detail/sp/800-177/final

- NIST SP 800-45 – Guidelines on Electronic Mail Security:  
  https://csrc.nist.gov/publications/detail/sp/800-45/version-2/final

- SANS – Phishing and Email Security:  
  https://www.sans.org/security-awareness-training/phishing/

- Security Blue Team – Blue Team Skills Overview:  
  https://securityblue.team/certifications/
