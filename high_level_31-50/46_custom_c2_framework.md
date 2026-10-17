# 46 — Build a Minimal Custom C2 Framework and Test It Against Your Own EDR

## What to Do
Write a basic Command and Control framework from scratch — an agent that checks in with a server over HTTP/S, receives commands, and returns output. Keep it minimal. Then test whether your own EDR detects it, and iterate.

## Open Source Resources
- Sliver / Havoc (study their architecture, don't copy verbatim) — for design reference only
- Python or Go (the two most common languages for custom C2 agents)
- Wazuh or LimaCharlie (as your defending EDR)
- MITRE ATT&CK C2 techniques — attack.mitre.org/tactics/TA0011

## Tips
- Start with plaintext HTTP check-ins, then progressively add HTTPS, jitter, and user-agent blending.
- The goal is to understand what makes C2 traffic detectable, not to build a production-grade tool.
- Keep the entire test in an air-gapped lab VM — never test custom C2 on a real network.

## When It's Completed
Your agent checks in, receives and executes at least one command, returns output, and you've documented what your EDR flagged and what it missed.
