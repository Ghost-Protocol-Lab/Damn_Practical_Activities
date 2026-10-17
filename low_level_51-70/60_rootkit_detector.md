# 60 — Write a Basic Rootkit Detector / Integrity Checker for Your Own Machine

## What to Do
Write a script that baselines your system (running processes, loaded kernel modules, open ports, startup entries, and critical file hashes) and then detects deviations from that baseline on subsequent runs.

## Open Source Resources
- Python psutil (process and system information)
- AIDE (host-based intrusion detection) — aide.github.io
- Tripwire open source — github.com/Tripwire/tripwire-open-source
- rkhunter — rkhunter.sourceforge.net (as a reference to study and compare against)

## Tips
- Hash critical system binaries (ls, ps, netstat, find) on a known-clean system and store the hashes offline — comparing against this baseline is the core of the detector.
- Cross-check process lists from multiple sources (e.g., /proc and ps output) — a rootkit hides from one but can't always hide from both.
- Keep the baseline on a read-only medium or a separate system so a rootkit can't modify it.

## When It's Completed
Your script produces a baseline, detects at least one deliberate change you made (a new process, a modified binary hash, a new startup entry), and alerts on it clearly.
