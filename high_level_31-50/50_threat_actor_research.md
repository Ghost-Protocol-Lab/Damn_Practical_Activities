# 50 — Research a Threat Actor in Detail and Reproduce Their Techniques

## What to Do
Pick a documented APT or threat actor group (APT29, Lazarus, Scattered Spider, etc.), read everything publicly available about their TTPs, then reproduce their key techniques in an isolated lab environment using the MITRE ATT&CK navigator.

## Open Source Resources
- MITRE ATT&CK Groups — attack.mitre.org/groups
- Mandiant / Google Threat Intelligence blog (free reports)
- Securelist by Kaspersky (detailed APT reports)
- Atomic Red Team (pre-built technique simulations)
- ATT&CK Navigator — mitre-attack.github.io/attack-navigator

## Tips
- Start with a group that has extensive public reporting (APT29 or Lazarus have years of detailed analysis).
- Map every reported technique to an ATT&CK ID, then use Atomic Red Team to simulate as many as possible in your lab.
- The goal is understanding their thinking, not just their tools — read the "why" behind each technique choice.

## When It's Completed
You've produced an ATT&CK Navigator layer for the group, simulated at least 5 of their techniques in a lab, and written a one-page summary of their operational style and what makes them distinct.
