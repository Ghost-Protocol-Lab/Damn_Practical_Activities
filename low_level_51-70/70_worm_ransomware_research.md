# 70 — Conduct Secured Research on Self-Replicating Worms, Ransomware, or Kernel Rootkits

## What to Do
In a fully isolated lab environment, study the code and behavior of documented malware in one of these advanced categories — understanding their replication logic, encryption scheme, or kernel-level hooking — without running live samples outside a controlled sandbox.

## Open Source Resources
- theZoo — github.com/ytisf/theZoo (academic malware samples, handle with extreme care)
- vx-underground — vx-underground.org (malware papers and source archives)
- MalwareBazaar — bazaar.abuse.ch (for documented recent samples)
- Cuckoo Sandbox / Any.run (for safe behavioral analysis)
- Academic papers: "An Analysis of the WannaCry Ransomware" and similar published research

## Tips
- For this category specifically: read existing analysis reports before touching any samples. Understanding from a paper first is safer and often more educational than hands-on analysis.
- Kernel rootkit research should be done in a VM with snapshots — a kernel-level bug can corrupt the entire VM, not just crash a process.
- Treat every sample as live and dangerous even if labeled "defused" — always in an air-gapped VM, always with snapshots, always with network completely disabled.

## When It's Completed
You've produced a structured technical analysis of one sample or category, identifying its replication/encryption/hooking mechanism, IOCs, and MITRE ATT&CK mapping — sourced from sandbox output and published research, not guesswork.
