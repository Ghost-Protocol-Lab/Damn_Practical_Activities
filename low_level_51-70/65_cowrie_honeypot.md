# 65 — Set Up a Cowrie SSH Honeypot and Review a Week of Bot Interactions

## What to Do
Deploy Cowrie (a medium-interaction SSH/Telnet honeypot) on a cheap VPS with SSH exposed on port 22, let it run for a week, and analyze what automated scanners and human attackers tried to do once they logged in.

## Open Source Resources
- Cowrie — github.com/cowrie/cowrie
- Kippo-graph (for visualizing Cowrie logs)
- ELK stack (for ingesting and analyzing Cowrie JSON logs)
- Cowrie documentation — cowrie.readthedocs.io

## Tips
- Move your real SSH to a non-standard port before exposing port 22 to Cowrie, so you don't lock yourself out.
- The most interesting data is in the session logs — what commands attackers ran after logging in reveals their actual objectives.
- Watch for attackers downloading and running scripts — Cowrie captures the downloaded files for analysis.

## When It's Completed
You've run Cowrie for a full week and produced a summary report: total login attempts, top credentials tried, top commands run, and any files attackers downloaded.
