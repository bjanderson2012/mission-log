# Case-001 — Home Internet Outage Triage (LAN OK, WAN/ISP Down)

## Summary
- **Date:** 2025-12-23
- **Category:** Network (Connectivity / ISP outage)
- **Severity:** Medium (whole network impacted)
- **Status:** Monitoring / Pending provider restoration

## Symptoms
- Internet worked earlier, then stopped.
- Multiple devices affected (not limited to one device).

## Impact
- Devices could connect to local Wi-Fi/LAN, but had no internet access.
- Workaround available: **secondary internet source** (if needed).

## Environment (sanitized)
- **Client device:** Windows 11 laptop
- **Network:** Home router providing DHCP + DNS forwarding
- **Connection type:** Fiber ONT (wall unit) → router WAN

## Baseline Checks
- Confirmed ONT/router powered and cabled.
- ONT indicator lights appeared normal; Ethernet link activity present.
- Reboot attempted (router and ISP equipment power cycle performed during troubleshooting).

## Troubleshooting Steps (chronological)
1) **Verify LAN / router reachability**
- **Command:** `ping 192.168.x.1` (replace with your default gateway)
- **Result:** Success (0% loss, low latency)
- **Interpretation:** Local network path is healthy (client ↔ router OK)

2) **Verify client IP configuration**
- **Command:** `ipconfig /all`
- **Result:** Valid private IPv4 via DHCP; default gateway set; DNS set to router (e.g., `192.168.x.1`)
- **Interpretation:** Client network configuration is normal

3) **Test WAN reachability by IP (bypass DNS)**
- **Command:** `ping 8.8.8.8`
- **Result:** Failure (100% packet loss)
- **Interpretation:** Internet/WAN path not reachable (upstream issue)

4) **Test DNS resolution**
- **Command:** `nslookup google.com`
- **Result:** DNS query timed out (default DNS = router)
- **Interpretation:** DNS failing because router cannot reach upstream resolvers (consistent with WAN down)

5) **Check where the route fails**
- **Command:** `tracert 8.8.8.8`
- **Result:** Reaches local gateway; reaches first hop beyond gateway; then becomes unreachable beyond that
- **Interpretation:** Failure is upstream (outside local LAN)

6) **Provider confirmation**
- **Action:** Checked provider status/outage tool on cellular data
- **Result:** “Known outage” reported with an ETA window
- **Interpretation:** Confirms provider-side outage (or upstream routing issue)

## Findings (confirmed)
- LAN is working (router reachable; DHCP working).
- WAN is down (cannot reach public IP 8.8.8.8).
- DNS fails due to lack of upstream connectivity.
- Route fails beyond the local network boundary.
- Provider reports a known outage.

## Root Cause (best current conclusion)
- **Most likely cause:** Provider outage / upstream routing issue.
- **Evidence:** WAN unreachable by IP + tracert fails beyond first hop beyond gateway + provider “known outage” confirmation.

## Outcome / Next Steps
- **Resolution:** Await provider restoration.
- **Workaround:** Switch to secondary internet source if needed.

**Post-restore verification:**
- `ping 8.8.8.8` succeeds
- `nslookup google.com` succeeds
- Browsing works
- Optional: speed test and short stability check

## Prevent / Improve
- Request/confirm fiber line burial/protection if drop is exposed.
- Keep a backup connectivity option available for critical work periods.

## Evidence (sanitized)
- Command outputs captured (avoid screenshots with personal identifiers).
- If screenshots are used: crop/blur any phone #, address, account IDs, IMEI/serial, public IPs, traceroute hop details.
