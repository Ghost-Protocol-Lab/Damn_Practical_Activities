# 42 — Build a Centralised Log System and Evade It Through a Full Attack Chain

## What to Do
Set up a centralized SIEM (Wazuh, ELK, or Graylog) collecting logs from at least two sources (a VM and a firewall), then execute a full simulated attack chain and try to complete each stage without triggering a detection rule.

## Open Source Resources
- Wazuh — wazuh.com
- Elastic SIEM — elastic.co/security
- Graylog — graylog.org
- Sigma rules (for writing your own detections to test against) — github.com/SigmaHQ/sigma
- Atomic Red Team (test atomic attack techniques) — github.com/redcanaryco/atomic-red-team

## Tips
- Write your own Sigma detection rules first, then see if your attack triggers them — building the defense sharpens the offense.
- Focus on log-gap techniques: living off the land, clearing specific event IDs, slowing attack pace to blend with baseline.
- A detection miss is as useful as a detection hit — document both.

## When It's Completed
A full attack chain (recon → access → lateral movement → exfil) is logged in the SIEM, and you can point to which stages were detected and which stages slipped through, with reasoning.
