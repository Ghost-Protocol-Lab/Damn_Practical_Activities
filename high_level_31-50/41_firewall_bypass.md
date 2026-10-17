# 41 — Establish a Firewall and Try to Bypass It Through Obfuscation / Stealth

## What to Do
Set up a firewall (pfSense, ufw, or iptables) with restrictive outbound rules on a lab network, then attempt to tunnel traffic out through allowed ports or protocols — HTTPS tunneling, ICMP tunneling, or covert channels over DNS.

## Open Source Resources
- pfSense — pfsense.org (free)
- ncat / socat (tunneling tools)
- Ptunnel (ICMP tunneling)
- Chisel (HTTP tunneling — github.com/jpillora/chisel)

## Tips
- Set your rules to only allow DNS (port 53) and HTTPS (port 443) outbound, and then try to exfil data over both channels.
- Log everything on the firewall side and review the logs after each bypass attempt.
- The most realistic bypass is traffic that looks exactly like normal HTTPS to a legitimate cloud provider.

## When It's Completed
You've successfully tunneled traffic past your own firewall rules using at least one technique, and documented how a firewall rule change would have blocked it.
