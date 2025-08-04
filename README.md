# Splunk SIEM Detection Lab

This project simulates a mini-SOC environment using Splunk for ingesting, parsing, and detecting malicious activity from log data. Built to demonstrate blue team competencies such as detection engineering, log analysis, and alerting based on Windows security event logs.

## 📌 Purpose

To build hands-on blue team experience by using Splunk to:
- Ingest and parse real Windows Event Logs
- Create detection rules using SPL (Search Processing Language)
- Analyze brute-force attempts, scanning behavior, and privilege escalation events
- Document findings in a structured, professional format

## 🔧 What’s Included

- `logs/`: Sample log files (e.g., Windows Security events)
- `detections/`: SPL queries to detect malicious patterns
- `screenshots/`: (To be added) Example detections and dashboards
- `README.md`: You’re reading it!

## 🛠️ Tools Used

- Splunk Free Edition (local instance)
- SPL (Search Processing Language)
- Sample logs from simulated Windows environment

## 🔍 Example Detections

- **Brute Force Detection:**
  Repeated failed logon attempts from a single IP/Machine.

- **Lateral Movement Attempt:**
  Unexpected `NTLM` or `Kerberos` authentications.

- **Privilege Escalation Attempt:**
  Usage of `whoami /priv` or suspicious group membership changes.

*(See full SPL queries in `/detections`)*

## 📖 Learning Outcomes

- Real-world SIEM experience (splunkd, parsing, indexing)
- Detection engineering basics using SPL
- Understanding of Windows event log taxonomy (Event ID 4624, 4625, etc.)
- Git and project documentation best practices

## ⚠️ Disclaimer

Logs used in this project are sanitized and do not contain real-world PII or production data. This is for educational and demonstrative purposes only.

## 💡 Next Steps

- Add more data sources (Linux logs, firewall, etc.)
- Build dashboard panels
- Integrate alert actions (e.g., email, webhook)

---

