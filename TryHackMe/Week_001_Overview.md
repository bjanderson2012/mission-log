# Advent of Cyber 2025 — Week 1 Summary

**Brian Anderson — TryHackMe Advent of Cyber 2025 (Days 1–7)**  
Hands-on cybersecurity training covering reconnaissance, web exploitation, file analysis, networking, and service enumeration.

---

## Overall Focus of Week 1
Week 1 built foundational offensive and defensive security skills through progressively more complex challenges:

- Investigating malicious emails
- Analyzing suspicious processes
- Debugging Python-based malware
- Extracting data from Windows systems
- Exploring Linux environments
- Performing structured network enumeration
- Interacting with live services (FTP, custom TCP, DNS, MySQL)

Each challenge reinforced core attacker methodology and defender-oriented investigation workflows.

---

## Daily Breakdown

### Day 1 — Email Investigation
**Skills practiced**
- Email header analysis
- Identifying suspicious domains
- Tracing sender infrastructure
- Inspecting phishing payloads

**Takeaway:** Email metadata often reveals malicious intent before a payload executes.

---

### Day 2 — Process Analysis & Malware Behavior
**Skills practiced**
- Inspecting Linux processes
- Observing anomalies in runtime behavior
- Identifying persistence techniques

**Takeaway:** Process monitoring exposes early signs of compromise.

---

### Day 3 — Python Malware Debugging
**Skills practiced**
- Reading and executing Python code
- Identifying malicious logic
- Reversing simple obfuscation

**Takeaway:** Even minimal scripts can hide harmful behavior. Code review is essential.

---

### Day 4 — Windows Forensics
**Skills practiced**
- Navigating Windows user directories
- Extracting evidence from browser artifacts
- Interpreting file-based activity

**Takeaway:** Forensic artifacts tell the true story of user activity.

---

### Day 5 — Linux Systems & Users
**Skills practiced**
- Linux filesystem navigation
- Permission structures
- Locating attacker-interest files

**Takeaway:** Misunderstanding Linux basics creates exploitable weaknesses.

---

### Day 6 — Network Fundamentals Introduction
**Skills practiced**
- Understanding ports and services
- Basic discovery of exposed endpoints
- Applying the enumeration mindset

**Takeaway:** Every open port is a potential entry point — or a clear warning sign.

---

### Day 7 — Full-Scope Enumeration & Multi-Service Interaction
**Tools used:** `nmap`, `ftp`, `nc`, `dig`, `ss`, `mysql`

**Accomplished**
- Performed targeted and full-range TCP/UDP scanning
- Identified services (FTP, custom TCP service, DNS)
- Retrieved Key 1 via anonymous FTP
- Retrieved Key 2 via custom TCP service
- Retrieved Key 3 from DNS TXT records
- Logged into QA console and enumerated active services
- Accessed MySQL backend and extracted final flag

**Takeaway:** A complete mini kill chain: **Recon → Access → Enumeration → Pivot → Data Extraction**

---

## Technical Themes Strengthened
- **Enumeration discipline:** Finding everything exposed, not just the obvious
- **File analysis:** Python scripts, Windows artifacts, Linux host files
- **Service interaction:** FTP, DNS, MySQL, custom TCP
- **Defensive awareness:** Recognizing misconfigurations and exposure points
- **Terminal confidence:** Command-line troubleshooting and corrective workflow

---

## Week 1 Status
- Days 1–7 completed
- Multi-service enumeration performed
- Host-level investigation performed
- Fundamentals established; investigation mindset forming
