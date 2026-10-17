# 57 — Make a Disk Image of Your Drive and Analyse It Completely

## What to Do
Create a forensic image of a drive (your own, or a spare), mount it read-only, and perform a full forensic analysis — deleted files, partition structure, file timeline, browser artifacts, and unallocated space.

## Open Source Resources
- Autopsy (forensic GUI built on Sleuth Kit) — autopsy.com
- The Sleuth Kit (CLI forensics tools) — sleuthkit.org
- dd or dcfldd (imaging tools)
- TestDisk / PhotoRec (deleted file recovery)
- Eric Zimmerman's forensic tools — ericzimmerman.github.io

## Tips
- Always image to a separate drive and mount the image read-only — never analyze the live disk directly.
- Use Autopsy's ingest modules to automate artifact extraction (browser history, recent files, email) before doing manual analysis.
- Check unallocated space and $Recycle.Bin for deleted artifacts — they're often still recoverable.

## When It's Completed
You've produced a forensic timeline, recovered at least one deleted file, and identified three categories of forensic artifacts (browser history, recent docs, login events) from the image.
