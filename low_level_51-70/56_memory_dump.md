# 56 — Take a Memory Dump of Your Computer and Analyse It

## What to Do
Capture a full RAM dump of your own running machine and analyze it for running processes, network connections, injected code, encryption keys, and any artifacts left behind by tools you deliberately ran beforehand as test markers.

## Open Source Resources
- Volatility 3 (memory forensics framework) — github.com/volatilityfoundation/volatility3
- WinPmem (Windows memory acquisition) — github.com/Velocidex/WinPmem
- LiME (Linux Memory Extractor) — github.com/504ensicsLabs/LiME
- MemProcFS (mount a memory image as a filesystem) — github.com/ufrisk/MemProcFS

## Tips
- Capture the dump as fast as possible after a known state — memory is volatile and changes constantly.
- Run Volatility plugins in order: pslist → netscan → malfind → dlllist. This gives you processes, connections, injected regions, and loaded libraries.
- Deliberately run something unusual before dumping (a known tool, a fake "malicious" process name) and see if you can find it in the dump.

## When It's Completed
You've extracted a process list, active network connections, and at least one artifact you planted deliberately, and documented the Volatility commands used for each.
