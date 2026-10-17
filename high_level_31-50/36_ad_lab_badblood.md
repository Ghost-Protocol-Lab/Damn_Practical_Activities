# 36 — Build an AD Lab with BadBlood + GOAT and Solve It

## What to Do
Spin up a Windows Active Directory lab using BadBlood (to populate it with realistic misconfigured users, groups, and ACLs) and GOAT (Guided Offensive Active Directory Training). Attack the environment using standard AD attack chains.

## Open Source Resources
- BadBlood — github.com/davidprowe/BadBlood
- GOAT (Guided Offensive AD Training) — github.com/Orange-Cyberdefense/GOAD
- BloodHound / SharpHound — for attack path visualization
- Impacket — for executing attacks from Linux

## Tips
- Run everything in VirtualBox or VMware on an isolated host-only network — AD labs should never have internet access.
- Let BloodHound map the environment first before attacking manually, so you understand the full attack surface.
- Try Kerberoasting, AS-REP roasting, and ACL abuse paths specifically — these are the most common in real engagements.

## When It's Completed
You've achieved Domain Admin via at least two different attack paths, and documented the kill chain for each one.
