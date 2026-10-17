# 32 — Recreate a Recent CVE from Scratch

## What to Do
Pick a CVE from the last 12 months that has a public advisory but no published PoC yet (or one where you want to understand the underlying mechanism). Set up a vulnerable environment and reproduce it yourself from the description alone.

## Open Source Resources
- NVD (nvd.nist.gov) — start here for CVE details
- VulnDB / Packet Storm for advisories
- ExploitDB — exploit-db.com
- GitHub for patched-vs-vulnerable diffs of affected projects

## Tips
- Binary-diffing the patch (using diaphora or bindiff) against the vulnerable version is often the fastest path to understanding what changed and why.
- Spin the vulnerable version in a VM so there's no risk to your real system.
- Focus on understanding the root cause, not just running the exploit.

## When It's Completed
You've reproduced the vulnerability in a controlled lab environment and can explain the root cause, the patch, and one mitigation in your own words.
