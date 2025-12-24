# Portfolio (Proof of Work)

This folder contains **recruiter-facing artifacts**: short case notes, runbooks, and templates that show how I troubleshoot, document, and think through issues.  
(Training notes and lab writeups live in `../TryHackMe/`.)

## What’s inside
- `Case_Notes/` — 1-page ticket-style case notes (sanitized)
- `Runbooks/` — short, repeatable troubleshooting playbooks
- `Templates/` — reusable templates/checklists for writing consistent notes

## Best artifacts (start here)
- **Case Note:** [Case-001 — Home Internet Outage Triage](Case_Notes/case-001-home-internet-outage-triage.md)
- **Runbook:** [Basic Network Troubleshooting Ladder](Runbooks/runbook-basic-network-troubleshooting-ladder.md)
- **Template:** [Ticket-Style Case Note Template](Templates/template-ticket-case-note.md)
- **Sanitization:** [Sanitization Checklist](Templates/sanitization-checklist.md)

## Case note standards (keeps it real)
- Max **1 page**
- **Chronological** steps (test → result → interpretation)
- Clear conclusion + next steps (fix / workaround / escalate)
- **Evidence > claims** (only write what was verified)

## Sanitization rules (non-negotiable)
Do **not** include:
- Names, addresses, phone numbers, email addresses
- Account/order/ticket numbers, billing details
- IMEI/serial/device IDs
- Wi-Fi SSIDs/passwords
- MAC addresses
- Public IP addresses or identifiable traceroute hop details

Prefer:
- Typed summaries over screenshots
- Placeholders like `192.168.x.x`, `ISP-A/ISP-B`, `router/gateway`

## Naming conventions
- Case notes: `case-###-short-title.md`
- Runbooks: `runbook-topic.md`
- Templates: `template-name.md`
