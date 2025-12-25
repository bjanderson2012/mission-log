# Advent of Cyber 2025 — Week 4 Summary (Days 22–24)

## Overview
Week 4 moved into practical detection, cloud enumeration, and raw HTTP mechanics. The theme was learning how real workflows chain: capture evidence → reduce noise → pivot → verify.

## Daily Highlights

### Day 22 — Network C2 Hunting (Zeek + RITA)
- Converted PCAP → Zeek logs, then used RITA to triage beaconing/C2-like patterns
- Looked for unusual TLS/client fingerprints, long-lived connections, odd ports, and repeat timing patterns

**Key Insight:**
Traffic analysis is about reduction: turn “too much data” into a short list of leads you can prove or disprove.

### Day 23 — AWS Enumeration + Privilege Discovery (AWS CLI)
- Confirmed identity and enumerated permissions (STS identity, IAM discovery, policy review)
- Identified a role trust path (`sts:AssumeRole`) and pivoted into it
- Enumerated allowed S3 access and retrieved the target file and flag

**Key Insight:**
Cloud compromise often follows a simple path: enumerate → find trust/roles → assume role → access resources.

### Day 24 — HTTP from the Command Line (cURL)
- Practiced HTTP actions with curl: GET/POST, response headers (`-i`)
- Worked with sessions/cookies by saving and replaying cookie jars
- Automated repeated requests with simple bash loops (wordlist-style testing)

**Key Insight:**
Web “state” (cookies/sessions/headers) is the difference between a one-off request and a real authenticated workflow.

## Tools & Commands Used
- **Zeek / RITA:** PCAP → logs, beaconing triage
- **AWS CLI:** identity + enumeration + role assumption + S3 access
- **cURL:** requests, headers, cookies/sessions; simple bash automation

## Takeaways
- Better understanding of how detection triage works (PCAP → logs → leads)
- Clearer mental model of IAM roles/trust paths and why assume-role matters
- Stronger grasp of HTTP state: headers, cookies, and session handling

## Coverage
Days 22–24 (Advent of Cyber 2025)
