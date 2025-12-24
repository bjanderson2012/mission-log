\# Runbook — Basic Network Troubleshooting Ladder (Home / Small Office)



\## Goal

Quickly determine where the failure is: device, LAN/router, DNS, or ISP/WAN.



\## Step 0 — Confirm scope

\- One device or multiple devices?

\- Wi-Fi only, or Wi-Fi + wired?

\- Any recent changes (router reboot, firmware update, new VPN)?



\## Step 1 — Local network (LAN)

1\) Find default gateway  

\- Windows: `ipconfig` → \*\*Default Gateway\*\*



2\) Ping the gateway  

\- `ping <gateway>` (example: `ping 192.168.x.1`)  

\- If this fails: local Wi-Fi/Ethernet/router issue.



\## Step 2 — Internet reachability by IP (WAN)

\- `ping 8.8.8.8` (or `ping 1.1.1.1`)  

\- If gateway ping works but this fails: WAN/ISP/ONT/modem issue.



\## Step 3 — DNS (name resolution)

\- `nslookup google.com`  

\- If IP ping works but DNS fails: DNS issue (router forwarding or configured resolvers).



\## Step 4 — Path visibility (where it dies)

\- `tracert 8.8.8.8`  

\- Useful to show whether failure occurs at gateway vs upstream.



\## Quick interpretations

\- Gateway ping fails → device/Wi-Fi/router problem  

\- Gateway ping ok, IP ping fails → ISP/WAN problem  

\- IP ping ok, DNS fails → DNS problem



\## What to capture (ticket notes)

\- Start time + scope (who/what affected)

\- Tests + results in order

\- Any outage confirmation from provider (if checked)

\- Workarounds used (hotspot/backup link)



