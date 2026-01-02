# Common Attack Patterns in Network Traffic

Many attacks exhibit recognizable network patterns. Understanding these patterns helps SOC analysts quickly identify threats.

---

## 🔍 Common Malicious Patterns

Typical indicators include:

- Beaconing behavior (regular interval connections)
- DNS tunneling
- Suspicious HTTP user agents
- Encrypted traffic to unknown endpoints
- Lateral movement via internal connections

---

## 🧠 Detection Considerations

Analysts should:

- Look for consistency and repetition
- Correlate with endpoint or authentication logs
- Validate findings with Threat Intelligence

---

## 📌 Key Takeaway

Recognizing patterns accelerates detection and reduces investigation time.

---

## 🔗 References

- MITRE ATT&CK – Network-Based Techniques:  
  https://attack.mitre.org/

- SANS – Detecting C2 Traffic:  
  https://www.sans.org/blog/detecting-command-and-control-traffic/
