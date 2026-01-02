# Memory Forensics Concepts

Memory forensics focuses on the analysis of **volatile memory (RAM)** to identify active or recently executed malicious activity.

It is especially useful for detecting threats that do not leave strong disk artifacts.

---

## 🎯 Why Memory Forensics Matters

Memory analysis can reveal:

- Running processes
- Network connections
- Loaded modules
- In-memory malware
- Command-line arguments

---

## 🧠 SOC-Level Memory Analysis

In BTL1 and entry-level SOC contexts, memory forensics focuses on:

- Understanding what data is available in memory
- Recognizing suspicious patterns
- Supporting alert validation

Advanced reverse engineering is **out of scope**.

---

## 📌 Key Takeaway

Memory forensics provides **real-time visibility** into system behavior during or after an incident.

---

## 🔗 References

- NIST SP 800-86 – Digital Forensics Guide:  
  https://csrc.nist.gov/publications/detail/sp/800-86/final

- SANS – Memory Forensics Concepts:  
  https://www.sans.org/blog/memory-forensics/
