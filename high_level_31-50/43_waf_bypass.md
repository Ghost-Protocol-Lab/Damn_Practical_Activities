# 43 — Establish a Web Application Firewall and Try to Bypass It

## What to Do
Deploy a WAF (ModSecurity with OWASP Core Rule Set, or Cloudflare's free tier in front of a local app) protecting a vulnerable app, then attempt to land SQL injection, XSS, and command injection payloads past it using encoding and bypass techniques.

## Open Source Resources
- ModSecurity + OWASP CRS — coreruleset.org
- DVWA or Juice Shop (as your target behind the WAF)
- WAFNinja (WAF bypass tool) — github.com/khalilbijjou/WAFNinja
- PayloadsAllTheThings WAF bypass section — github.com/swisskyrepo/PayloadsAllTheThings

## Tips
- Start with completely unobfuscated payloads so you know the WAF is working, then incrementally add encoding.
- Try both signature-based bypasses (encoding tricks) and logic bypasses (breaking the parsing logic).
- Document every payload variant and whether it was blocked, flagged, or passed.

## When It's Completed
At least one payload class (e.g., SQLi or XSS) has a working bypass documented, and you've written the WAF rule that would have caught it.
