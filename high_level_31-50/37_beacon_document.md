# 37 — Create a Document with a Beacon and Monitor Hits

## What to Do
Embed a tracking beacon (a hidden web bug — a 1x1 image or DNS-based callback) inside a document you control, share it with yourself or a consenting friend, and observe when and where it's opened.

## Open Source Resources
- Canarytokens — canarytokens.org (free, legitimate beacon service for exactly this use case)
- Grabify (for URL-based tracking tokens — link only, no malware)
- Burp Collaborator for DNS/HTTP callback tracking

## Tips
- Canarytokens is the cleanest option — it's purpose-built for this, free, and requires no infrastructure of your own.
- Only send the beacon to people who know and have consented to being part of the test.
- Note the metadata that comes back: IP, user agent, approximate location, time — this is exactly what a real attacker sees.

## When It's Completed
The beacon has been triggered and you've received and logged at least one callback with associated metadata.
