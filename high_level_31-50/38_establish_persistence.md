# 38 — Establish Persistence on Your Own or a Friend's Machine (With Permission)

## What to Do
After gaining access to a machine you own or have explicit written permission to test, establish a persistent foothold that survives a reboot — a scheduled task, a startup entry, a rogue service, or a registry run key — then document how to detect and remove it.

## Open Source Resources
- MITRE ATT&CK Persistence techniques — attack.mitre.org (TA0003)
- Metasploit Framework persistence modules
- SysinternalsAutoRuns — for detecting your own implant afterward

## Tips
- Always test the detection side too — set up Autoruns or a log monitor and see if your persistence method shows up.
- Use the least-obvious persistence method you know, then challenge yourself to find it using only defensive tooling.
- Document the full install and remove procedure before deploying, so you can clean up completely.

## When It's Completed
Persistence survives at least one reboot, you've confirmed it's running, and you've fully removed it and verified removal.
