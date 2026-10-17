# 45 — Map Your Workplace or University Network from the Inside

## What to Do
From inside the network (connected to the org's Wi-Fi or LAN, with permission), perform internal network discovery: active hosts, services, OS fingerprinting, and any internal resources visible to your user account.

## Open Source Resources
- Nmap — nmap.org
- Netdiscover (ARP scanning for local host discovery)
- Nessus Essentials (free tier, up to 16 IPs)
- BloodHound (if Windows AD is in scope)

## Tips
- Get written permission — internal scanning without it is a serious policy violation even if you work there.
- Start with ARP discovery before any port scanning to avoid being noisy.
- Map what a regular user account can reach versus what an admin would see — the gap is often revealing.

## When It's Completed
You've produced a network map with all discovered hosts, open services, and at least one finding that the IT team didn't know was visible to regular users.
