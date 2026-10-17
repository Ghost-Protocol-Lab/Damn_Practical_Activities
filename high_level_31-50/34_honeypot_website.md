# 34 — Set Up a Honeypot Vulnerable Website and Monitor Hits

## What to Do
Deploy a deliberately vulnerable web app (DVWA, Juice Shop, or a custom one) on a VPS with logging enabled. Leave it running and observe how quickly automated scanners and real attackers find and probe it.

## Open Source Resources
- DVWA — github.com/digininja/DVWA
- OWASP Juice Shop — github.com/juice-shop/juice-shop
- T-Pot honeypot platform — github.com/telekom-security/tpotce
- GoAccess or ELK for log visualization

## Tips
- Never put real data or credentials anywhere on the honeypot server.
- Use a VPS you don't care about, fully isolated from your real infrastructure.
- Set up logging before exposing it — you want data from the first probe, not after you noticed traffic.

## When It's Completed
The honeypot has run for at least a week, and you've produced a report of what hit it: scan types, IP origins, payloads attempted, and what the attacker appeared to be after.
