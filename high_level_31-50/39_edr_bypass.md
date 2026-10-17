# 39 — Establish an EDR and Try to Bypass It with Obfuscation

## What to Do
Install a free or trial EDR (Elastic, Wazuh, LimaCharlie) on a lab VM, then attempt to execute known-bad tooling (in a fully isolated environment) in a way that evades detection using obfuscation and staging techniques.

## Open Source Resources
- Wazuh (free, open source EDR/SIEM) — wazuh.com
- LimaCharlie (free tier) — limacharlie.io
- Elastic Security (free tier)
- AMSI bypass research — github.com
- Sliver or Havoc C2 frameworks (for test payloads in isolated labs only)

## Tips
- Change one variable at a time (encoding, staging, process injection) so you can isolate what the EDR actually detects.
- Keep the entire test inside a host-only VM with no internet access.
- Write down what the EDR caught and what it missed — the "miss" list is as valuable as the "catch" list.

## When It's Completed
You've documented at least three obfuscation techniques — which ones triggered the EDR, which ones didn't, and a hypothesis for why.
