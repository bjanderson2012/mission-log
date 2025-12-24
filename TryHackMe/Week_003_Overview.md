\# TryHackMe — Advent of Cyber (Week 3 Summary)

\*\*Days 15–21 | Brian Anderson\*\*



\## Overview



Week 3 focused on investigation workflows across log# TryHackMe — Advent of Cyber (Week 3 Summary)

\*\*Days 15–21 | Brian Anderson\*\*



\## Overview



Week 3 focused on investigation workflows across logs, Windows artifacts, decoding/obfuscation, web exploitation mechanics, and ICS/SCADA fundamentals. The consistent theme was building a repeatable analyst rhythm: collect evidence → transform/replay → verify findings.



---



\## Daily Highlights



\### Day 15 — Splunk Investigation (Logs + Telemetry)

\- Pivoted between Apache logs and Sysmon telemetry

\- Decoded payloads and reconstructed an attack chain



\*\*Key Insight:\*\*  

Cross-source pivoting (web logs + endpoint telemetry) accelerates attribution and timeline clarity.



---



\### Day 16 — Windows Registry Forensics

\- Worked with registry hives/keys

\- Used Registry Editor and Registry Explorer workflows



\*\*Key Insight:\*\*  

The registry is a high-signal artifact source for persistence and system context.



---



\### Day 17 — CyberChef + Encoding/Decoding + HTTP Header Clues

\- Performed multi-step decode workflows using CyberChef

\- Used HTTP header clues to guide transformations

\- Learned to be precise with “recipe” sequencing



\*\*Key Insight:\*\*  

Small decode mismatches can derail the entire chain — accuracy and validation matter.



---



\### Day 18 — PowerShell Obfuscation Reversal

\- Reversed obfuscation using CyberChef steps (e.g., Base64/XOR/hex)

\- Focused on understanding the script’s real behavior



\*\*Key Insight:\*\*  

Obfuscation is usually layered. The goal is clarity: what it does, how it does it, and why it matters.



---



\### Day 19 — ICS/SCADA + Modbus Basics

\- Practiced Modbus reads/writes using Python (`pymodbus`)

\- Followed safe remediation order: read state → change → verify



\*\*Key Insight:\*\*  

In ICS environments, verification and safe sequencing matter as much as technical ability.



---



\### Day 20 — Race Conditions (Concurrency)

\- Used Burp Proxy/HTTP history to understand application flow

\- Used Repeater to send parallel requests and observe concurrency impact

\- Demonstrated overselling stock via race condition behavior



\*\*Key Insight:\*\*  

Race conditions are not “magic” — they’re reproducible timing failures revealed with controlled parallelism.



---



\### Day 21 — HTA Reverse Engineering (Static Analysis)

\- Performed static analysis of an HTA file

\- Reviewed metadata, functions, network indicators, encoding/obfuscation, and potential exfiltration behavior



\*\*Key Insight:\*\*  

Static analysis starts with structure and indicators: what it calls, what it reaches, and what it tries to hide.



---



\## Tools Used



\- \*\*Splunk\*\*

\- \*\*Burp Suite:\*\* Proxy, Repeater

\- \*\*CyberChef\*\*

\- \*\*Python + `pymodbus`\*\*

\- \*\*Windows Registry Tools:\*\* Registry Editor, Registry Explorer

\- \*\*Linux workflow:\*\* file viewing/editing (nano/pluma), running scripts



---



\## What Was Hardest



\- Multi-step decoding where a small mismatch breaks everything (CyberChef recipe variations)

\- Instances where values differed from walkthroughs, requiring trust in recon outputs



---



\## What Clicked



\- A repeatable investigation rhythm: \*\*observe → extract artifact/request/data → replay/transform → verify\*\*

\- Burp as a “see what’s happening on the wire” tool, not just an attack tool

\- In ICS labs: \*\*read state first, change in safe order, verify after\*\*



---



\## Status



✔ Week 3 complete (Days 15–21)  

➡ Ready to begin Week 4 / Day 22

s, Windows artifacts, decoding/obfuscation, web exploitation mechanics, and ICS/SCADA fundamentals. The consistent theme was building a repeatable analyst rhythm: collect evidence → transform/replay → verify findings.



---



\## Daily Highlights



\### Day 15 — Splunk Investigation (Logs + Telemetry)

\- Pivoted between Apache logs and Sysmon telemetry

\- Decoded payloads and reconstructed an attack chain



\*\*Key Insight:\*\*  

Cross-source pivoting (web logs + endpoint telemetry) accelerates attribution and timeline clarity.



---



\### Day 16 — Windows Registry Forensics

\- Worked with registry hives/keys

\- Used Registry Editor and Registry Explorer workflows



\*\*Key Insight:\*\*  

The registry is a high-signal artifact source for persistence and system context.



---



\### Day 17 — CyberChef + Encoding/Decoding + HTTP Header Clues

\- Performed multi-step decode workflows using CyberChef

\- Used HTTP header clues to guide transformations

\- Learned to be precise with “recipe” sequencing



\*\*Key Insight:\*\*  

Small decode mismatches can derail the entire chain — accuracy and validation matter.



---



\### Day 18 — PowerShell Obfuscation Reversal

\- Reversed obfuscation using CyberChef steps (e.g., Base64/XOR/hex)

\- Focused on understanding the script’s real behavior



\*\*Key Insight:\*\*  

Obfuscation is usually layered. The goal is clarity: what it does, how it does it, and why it matters.



---



\### Day 19 — ICS/SCADA + Modbus Basics

\- Practiced Modbus reads/writes using Python (`pymodbus`)

\- Followed safe remediation order: read state → change → verify



\*\*Key Insight:\*\*  

In ICS environments, verification and safe sequencing matter as much as technical ability.



---



\### Day 20 — Race Conditions (Concurrency)

\- Used Burp Proxy/HTTP history to understand application flow

\- Used Repeater to send parallel requests and observe concurrency impact

\- Demonstrated overselling stock via race condition behavior



\*\*Key Insight:\*\*  

Race conditions are not “magic” — they’re reproducible timing failures revealed with controlled parallelism.



---



\### Day 21 — HTA Reverse Engineering (Static Analysis)

\- Performed static analysis of an HTA file

\- Reviewed metadata, functions, network indicators, encoding/obfuscation, and potential exfiltration behavior



\*\*Key Insight:\*\*  

Static analysis starts with structure and indicators: what it calls, what it reaches, and what it tries to hide.



---



\## Tools Used



\- \*\*Splunk\*\*

\- \*\*Burp Suite:\*\* Proxy, Repeater

\- \*\*CyberChef\*\*

\- \*\*Python + `pymodbus`\*\*

\- \*\*Windows Registry Tools:\*\* Registry Editor, Registry Explorer

\- \*\*Linux workflow:\*\* file viewing/editing (nano/pluma), running scripts



---



\## What Was Hardest



\- Multi-step decoding where a small mismatch breaks everything (CyberChef recipe variations)

\- Instances where values differed from walkthroughs, requiring trust in recon outputs



---



\## What Clicked



\- A repeatable investigation rhythm: \*\*observe → extract artifact/request/data → replay/transform → verify\*\*

\- Burp as a “see what’s happening on the wire” tool, not just an attack tool

\- In ICS labs: \*\*read state first, change in safe order, verify after\*\*



---



\## Status



✔ Week 3 complete (Days 15–21)  

➡ Ready to begin Week 4 / Day 22



