\# TryHackMe — Advent of Cyber (Week 2 Summary)

\*\*Days 8–14 | Brian Anderson\*\*



\## Overview



Week 2 expanded beyond basic enumeration into applied security concepts across AI misuse, cryptography, web vulnerabilities, detection engineering, and container security. The focus shifted toward understanding \*why\* attacks work, not just how to execute them.

\# TryHackMe — Advent of Cyber (Week 2 Summary)

\*\*Days 8–14 | Brian Anderson\*\*



\## Overview



Week 2 expanded beyond basic enumeration into applied security concepts across AI misuse, cryptography, web vulnerabilities, detection engineering, and container security. The focus shifted toward understanding \*why\* attacks work, not just how to execute them.



---



\## Daily Highlights



\### Day 8 — Agentic AI \& Prompt Injection Concepts

\- Introduced agent-based AI workflows and tool-calling risks

\- Explored prompt injection and indirect control of AI agents

\- Built foundational awareness of AI misuse and escalation paths



\*\*Key Insight:\*\*  

AI agents amplify risk when they are trusted to act without strict boundaries.



---



\### Day 9 — Password-Based Encryption Attacks

\- Cracked password-protected ZIP and PDF files

\- Extracted hashes and performed dictionary attacks

\- Learned when to escalate to brute-force or mask-based attacks



\*\*Key Insight:\*\*  

Encryption often fails at the password layer — attackers crack credentials offline, not algorithms.



---



\### Day 10 — SIEM Concepts (Microsoft Sentinel)

\- Walked through alert triage and SOC workflows

\- Attempted hands-on lab but was blocked by Azure sandbox permissions and missing seeded alerts



\*\*Key Insight:\*\*  

Understanding detection logic and alert context matters even when labs fail operationally.



---



\### Day 11 — Cross-Site Scripting (XSS)

\- Tested basic XSS payloads

\- Distinguished reflected vs stored XSS

\- Reviewed prevention and input handling concepts



\*\*Key Insight:\*\*  

XSS is a trust failure — stored XSS increases impact due to persistence.



---



\### Day 12 — Phishing Analysis \& Classification

\- Analyzed headers and return-paths

\- Differentiated spoofing, impersonation, and social engineering

\- Practiced justification-based phishing triage



\*\*Key Insight:\*\*  

Naming the technique clarifies response and reduces false positives.



---



\### Day 13 — YARA Fundamentals

\- Wrote basic YARA rules

\- Used regex-based matching

\- Debugged issues related to spacing, casing, and rule logic



\*\*Key Insight:\*\*  

Detection engineering requires precision — small rule changes have large effects.



---



\### Day 14 — Containers \& Docker Misconfiguration

\- Explored container runtime behavior

\- Identified exposed Docker socket

\- Pivoted from container context to privileged access

\- Executed recovery script to restore services



\*\*Key Insight:\*\*  

Containers are not VMs — misconfiguration can collapse isolation boundaries.



---



\## Tools \& Commands Used



\- \*\*Password Cracking:\*\* `pdfcrack`, `zip2john`, `pdf2john`, `john`

\- \*\*Web Testing:\*\* Basic XSS payloads

\- \*\*Email Analysis:\*\* Header and return-path inspection

\- \*\*YARA:\*\* `yara -r -s`, rule debugging

\- \*\*Containers:\*\* `docker ps`, `docker exec`, socket inspection



---



\## Week 2 Takeaways



\- Stronger understanding of attacker tradecraft across domains

\- Improved confidence troubleshooting failed labs

\- Exposure to AI misuse, detection logic, and container risk

\- Growing ability to connect offensive techniques to defensive impact



---



\## Status



✔ Week 2 complete  

➡ Ready to begin Week 3 / Day 15



---



\## Daily Highlights



\### Day 8 — Agentic AI \& Prompt Injection Concepts

\- Introduced agent-based AI workflows and tool-calling risks

\- Explored prompt injection and indirect control of AI agents

\- Built foundational awareness of AI misuse and escalation paths



\*\*Key Insight:\*\*  

AI agents amplify risk when they are trusted to act without strict boundaries.



---



\### Day 9 — Password-Based Encryption Attacks

\- Cracked password-protected ZIP and PDF files

\- Extracted hashes and performed dictionary attacks

\- Learned when to escalate to brute-force or mask-based attacks



\*\*Key Insight:\*\*  

Encryption often fails at the password layer — attackers crack credentials offline, not algorithms.



---



\### Day 10 — SIEM Concepts (Microsoft Sentinel)

\- Walked through alert triage and SOC workflows

\- Attempted hands-on lab but was blocked by Azure sandbox permissions and missing seeded alerts



\*\*Key Insight:\*\*  

Understanding detection logic and alert context matters even when labs fail operationally.



---



\### Day 11 — Cross-Site Scripting (XSS)

\- Tested basic XSS payloads

\- Distinguished reflected vs stored XSS

\- Reviewed prevention and input handling concepts



\*\*Key Insight:\*\*  

XSS is a trust failure — stored XSS increases impact due to persistence.



---



\### Day 12 — Phishing Analysis \& Classification

\- Analyzed headers and return-paths

\- Differentiated spoofing, impersonation, and social engineering

\- Practiced justification-based phishing triage



\*\*Key Insight:\*\*  

Naming the technique clarifies response and reduces false positives.



---



\### Day 13 — YARA Fundamentals

\- Wrote basic YARA rules

\- Used regex-based matching

\- Debugged issues related to spacing, casing, and rule logic



\*\*Key Insight:\*\*  

Detection engineering requires precision — small rule changes have large effects.



---



\### Day 14 — Containers \& Docker Misconfiguration

\- Explored container runtime behavior

\- Identified exposed Docker socket

\- Pivoted from container context to privileged access

\- Executed recovery script to restore services



\*\*Key Insight:\*\*  

Containers are not VMs — misconfiguration can collapse isolation boundaries.



---



\## Tools \& Commands Used



\- \*\*Password Cracking:\*\* `pdfcrack`, `zip2john`, `pdf2john`, `john`

\- \*\*Web Testing:\*\* Basic XSS payloads

\- \*\*Email Analysis:\*\* Header and return-path inspection

\- \*\*YARA:\*\* `yara -r -s`, rule debugging

\- \*\*Containers:\*\* `docker ps`, `docker exec`, socket inspection



---



\## Week 2 Takeaways



\- Stronger understanding of attacker tradecraft across domains

\- Improved confidence troubleshooting failed labs

\- Exposure to AI misuse, detection logic, and container risk

\- Growing ability to connect offensive techniques to defensive impact



---



\## Status



✔ Week 2 complete  

➡ Ready to begin Week 3 / Day 15



