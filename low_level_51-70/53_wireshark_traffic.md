# 53 — Install Wireshark and Inspect Your Entire Traffic

## What to Do
Capture all traffic on your main network interface for a defined period and analyze what your devices are actually sending and receiving — which hosts they connect to, what protocols they use, and what (if any) unencrypted data is visible.

## Open Source Resources
- Wireshark — wireshark.org
- tcpdump (CLI capture, pairs well with Wireshark analysis)
- NetworkMiner (passive network forensics tool)
- Wireshark display filter reference — wiki.wireshark.org

## Tips
- Use capture filters to reduce noise: `port 80 or port 443` for web traffic, `not arp` to suppress ARP chatter.
- Look specifically for anything unencrypted (port 80, plain DNS, FTP) — these are the most immediately actionable findings.
- Check what your phone and smart devices are doing, not just your laptop.

## When It's Completed
You've captured at least 30 minutes of real traffic, identified every distinct external host your devices communicate with, and flagged anything that surprised you.
