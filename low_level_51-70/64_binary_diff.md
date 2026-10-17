# 64 — Binary-Diff a Patched vs Unpatched Version of an Open Source Tool

## What to Do
Download two consecutive versions of an open source tool where a security fix was made, binary-diff them to identify exactly what changed, and use that diff to understand (and if applicable, reproduce) the original vulnerability.

## Open Source Resources
- Diaphora (IDA/Ghidra binary diffing plugin) — github.com/joxeankoret/diaphora
- Bindiff (free version available from Google/Zynamics)
- diffoscope (source-level diff for packages) — diffoscope.org
- The project's git log and security advisory for ground truth

## Tips
- Use the git commit that fixed the bug as your guide — read it before diffing so you know what you're looking for.
- Focus on functions that changed, not the whole binary — Diaphora highlights changed functions directly.
- The shortest path from diff to understanding: read the advisory → find the changed function → read old vs new logic → identify the flaw.

## When It's Completed
You've identified the exact function and code change that fixed the vulnerability, and can explain the root cause in plain language from the binary diff alone.
