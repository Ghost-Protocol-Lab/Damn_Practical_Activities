# 48 — Explore LOLBins in a Windows VM and See What Your EDR Flags

## What to Do
In an isolated Windows lab VM, work through a selection of Living Off the Land Binaries — legitimate Windows tools abused for attacker purposes — and record which ones your EDR detects vs. silently allows.

## Open Source Resources
- LOLBAS Project — lolbas-project.github.io (the definitive LOLBins reference)
- Atomic Red Team — github.com/redcanaryco/atomic-red-team (pre-built LOLBin test cases)
- Wazuh or Elastic (as your EDR/SIEM)
- MITRE ATT&CK for corresponding technique IDs

## Tips
- Start with the most commonly abused ones: certutil, mshta, regsvr32, wmic, bitsadmin, rundll32.
- Run each one, then check your EDR dashboard immediately after — note whether it fired, the alert severity, and the technique ID.
- The goal is building a personal "detection gap" map for your specific EDR configuration.

## When It's Completed
You've run at least 10 LOLBin techniques, logged which triggered detections and which didn't, and written a one-line explanation of why each undetected one slipped through.
