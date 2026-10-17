# 47 — Try Domain Fronting or Traffic Shaping to Evade Your Own DLP / Logging

## What to Do
Attempt to disguise exfil traffic as legitimate cloud service traffic (domain fronting concept) or shape it to blend with normal baselines — slow exfil, chunked over long periods — and see if your SIEM or DLP picks it up.

## Open Source Resources
- Research papers on domain fronting (search "domain fronting cloudfront" academic papers)
- Cobalt Strike's malleable C2 profile documentation (for concept reference — you don't need CS itself)
- Scapy (for crafting and shaping packets in your lab)

## Tips
- Major CDNs have largely patched domain fronting, so this is a conceptual/lab exercise — focus on understanding why it worked and what detection it was designed to bypass.
- Slow exfil (a few KB per hour, mimicking telemetry) is harder to detect than a burst — test both.
- Build the detection rule after the bypass attempt, not before.

## When It's Completed
You've exfiltrated test data past your own defensive tools using at least one evasion technique and documented exactly which log entry (or lack thereof) revealed the gap.
