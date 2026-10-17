# 68 — Craft a Harmless File That Changes Its Own Hash Each Run and Test on VirusTotal

## What to Do
Write a benign program or script that produces a different file hash every time it runs (by appending a timestamp, random bytes, or recompiling itself) and submit several variants to VirusTotal to see how AV engines handle hash-based vs behavioral detection.

## Open Source Resources
- VirusTotal — virustotal.com (submission limit: 4 files/min on free tier)
- Python hashlib (for demonstrating hash changes)
- UPX packer (to study how packing changes signatures)
- YARA (write a behavioral rule that catches all variants regardless of hash)

## Tips
- Keep the program completely inert — no network connections, no file system writes outside its own directory, no process spawning.
- The goal is to understand the difference between static (hash/signature) detection and behavioral/heuristic detection.
- Write a YARA rule after submitting — challenge yourself to write one that catches all variants based on code patterns, not the hash.

## When It's Completed
You've submitted at least five hash-different variants, documented which engines flagged them despite the hash change (behavioral detection), and written a YARA rule that catches all variants.
