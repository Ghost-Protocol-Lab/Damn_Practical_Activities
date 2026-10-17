# 55 — Download a Firmware Sample and Do Forensics on It

## What to Do
Download publicly available firmware for a consumer device (router, IP camera, smart TV) from the manufacturer's site or firmware.re, extract the filesystem, and analyze its contents for hardcoded credentials, insecure services, and interesting binaries.

## Open Source Resources
- Binwalk (firmware extraction) — github.com/ReFirmLabs/binwalk
- firmware.re (online firmware analysis service)
- Firmwalker (automated firmware security scanner) — github.com/craigz28/firmwalker
- FACT (Firmware Analysis and Comparison Tool) — github.com/fkie-cad/FACT_core

## Tips
- Start with `binwalk -e` to extract, then `firmwalker` to automatically flag common issues (hardcoded passwords, private keys, insecure configs).
- Look at `/etc/shadow`, `/etc/passwd`, and any init scripts for hardcoded credentials.
- Compare two firmware versions (old vs. new) to see what a security patch actually fixed.

## When It's Completed
You've extracted the filesystem, identified at least two security concerns (hardcoded creds, insecure service, old vulnerable library), and documented their locations and severity.
