# 66 — Build a Keylogger and Info Stealer for Research and Test Against Defenses

## What to Do
Write a basic keylogger and credential-harvesting tool from scratch on a machine you own, purely to understand how they work and what defensive signatures they trigger. Test it against your own AV and EDR, then fully remove it.

## Open Source Resources
- Python pynput library (keyboard event hooking)
- Windows SetWindowsHookEx documentation (for understanding low-level hooking)
- Wazuh / Elastic (as your defensive layer to test against)
- MITRE ATT&CK T1056 (Input Capture technique reference)

## Tips
- Keep the tool entirely on your own machine — never run it on any system you don't own, and never exfiltrate actual keystrokes anywhere.
- Test against your EDR before and after obfuscating — note exactly which detection fires and what the alert says.
- Read the Windows API documentation for hooking, not just a tutorial — understanding the underlying API is the point.

## When It's Completed
You've built a working keylogger, tested which defensive tools detect it, applied at least one obfuscation technique, and fully removed it with verified cleanup.
