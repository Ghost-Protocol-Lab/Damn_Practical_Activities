# 58 — Do Registry Forensics on a Windows Laptop

## What to Do
Analyze the Windows registry hives (SYSTEM, SOFTWARE, NTUSER.DAT, SAM) for forensic artifacts: recently run programs, USB devices ever plugged in, installed software, user activity, and persistence mechanisms.

## Open Source Resources
- Registry Explorer (Eric Zimmerman) — ericzimmerman.github.io
- RegRipper — github.com/keydet89/RegRipper3.0
- ShimCacheParser (for application execution history)
- Windows Registry Forensics reference — forensicswiki.xyz

## Tips
- Focus on the most forensically rich keys first: NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Run (persistence), SYSTEM\CurrentControlSet\Enum\USBSTOR (USB history), and RecentDocs.
- Use Registry Explorer's bookmarks feature — it has pre-loaded views for common forensic artifacts.
- Export interesting keys before analysis so you have a reference copy.

## When It's Completed
You've identified every USB device ever connected to the machine, all persistence entries in run keys, and the 10 most recently executed applications — all from the registry alone.
