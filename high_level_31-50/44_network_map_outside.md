# 44 — Map Your Workplace or University Network from the Outside

## What to Do
Using only passive OSINT and active recon on infrastructure you have authorization to probe, build a map of your organization's externally visible attack surface: IP ranges, exposed services, subdomains, email infrastructure, and certificate data.

## Open Source Resources
- Shodan — shodan.io
- Censys — search.censys.io
- Amass (subdomain enumeration) — github.com/owasp-amass/amass
- DNSdumpster — dnsdumpster.com
- crt.sh (certificate transparency logs)

## Tips
- Get explicit permission from your IT/security team in writing before doing any active scanning.
- Passive sources (Shodan, crt.sh, WHOIS) are safer starting points — they don't touch the org's systems at all.
- Document what you find that the org might not know is exposed — that's the deliverable.

## When It's Completed
You've produced an external attack surface map with at least: all public IP ranges, exposed services, subdomains, and mail/DNS configuration — plus a list of anything that looks unintentionally exposed.
