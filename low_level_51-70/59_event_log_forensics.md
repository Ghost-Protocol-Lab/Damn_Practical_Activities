# 59 — Do Event Log Forensics on Your Own Laptop

## What to Do
Analyze your Windows or Linux system logs for forensic artifacts: logon/logoff events, privilege escalation, service installs, account changes, and process execution — as if you were investigating yourself.

## Open Source Resources
- Eric Zimmerman's EvtxECmd (Windows event log parser) — ericzimmerman.github.io
- Chainsaw (fast event log hunting) — github.com/WithSecureLabs/chainsaw
- Hayabusa (Windows event log threat hunting) — github.com/Yamato-Security/hayabusa
- Sigma rules (detection logic mapped to event IDs)

## Tips
- Key Windows event IDs to know by heart: 4624 (logon), 4625 (failed logon), 4672 (admin logon), 7045 (service install), 4698 (scheduled task created).
- Run Chainsaw with Sigma rules to get automated detections, then manually investigate the hits.
- Correlate event log timestamps with your own memory of what you were doing — it grounds abstract log analysis in reality.

## When It's Completed
You've identified your own logon history for the past week, found at least one interesting or unexpected event, and mapped it to its MITRE ATT&CK technique ID.
