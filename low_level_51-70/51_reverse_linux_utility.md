# 51 — Reverse Engineering a Linux Utility

## What to Do
Pick a compiled Linux binary you use regularly (ls, curl, ping, or any small open-source tool) and reverse-engineer it using static and dynamic analysis. Compare your findings against the source code afterward to validate your analysis.

## Open Source Resources
- Ghidra — ghidra-sre.org (NSA's free decompiler)
- Radare2 — rada.re (command-line reversing framework)
- GDB with PEDA/pwndbg plugin (dynamic analysis)
- Binary Ninja free tier — binary.ninja
- man pages and the actual source code (for comparison)

## Tips
- Start with a small, single-purpose utility (e.g., base64, xxd) before tackling anything complex.
- Use `file`, `strings`, `ldd`, and `nm` before opening a decompiler — gather as much info passively as possible first.
- Work function by function, not top to bottom — find main(), then follow the call graph outward.

## When It's Completed
You've identified the main logic flow, named at least five functions correctly, and cross-validated your decompiled output against the actual source.
