# 69 — Build a RAT / Backdoor or Cryptojacker or Adware for Study Purposes

## What to Do
Build one of these malware categories from scratch in a completely air-gapped lab, purely to understand how they work architecturally — their persistence, communication, and evasion mechanisms. Never deploy outside the lab.

## Open Source Resources
- MITRE ATT&CK (for the techniques each category uses)
- theZoo malware repository — github.com/ytisf/theZoo (for studying existing samples)
- Python or C (for writing your own minimal implementation)
- Any.run or Cuckoo Sandbox (for behavioral analysis of your own creation)

## Tips
- An air-gapped VM with no shared folders and no network adapter is the absolute minimum safety requirement — non-negotiable.
- Focus on one mechanism at a time: persistence first, then communication, then evasion. Understanding each piece separately is more valuable than a working end-to-end tool.
- After building, immediately analyze it with your own defensive tools — flip to the defender's perspective and see what signatures your creation leaves behind.

## When It's Completed
You've built a working minimal version in an isolated lab, analyzed it with a sandbox, identified every MITRE ATT&CK technique it uses, and documented the detection signatures it leaves behind.
