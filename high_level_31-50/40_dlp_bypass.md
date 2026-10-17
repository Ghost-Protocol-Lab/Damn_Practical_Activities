# 40 — Establish a DLP System and Try to Bypass It

## What to Do
Set up a Data Loss Prevention tool (MyDLP, OpenDLP, or a cloud-based free tier) and then attempt to exfiltrate a test "sensitive" file — using encoding, steganography, or DNS tunneling — and see what the DLP catches.

## Open Source Resources
- OpenDLP — github.com/ezarko/opendlp
- MyDLP (community edition)
- Iodine (DNS tunneling tool — lab use only)
- Steghide (steganography, hiding data in images)

## Tips
- Use clearly fake "sensitive" data (e.g., a file of dummy credit card numbers in Luhn-valid format) — never real PII.
- Try at least three exfil channels: HTTP, DNS, and a cloud storage upload.
- The goal is to understand where your DLP has blind spots, not just to beat it.

## When It's Completed
You've tested at least three exfil methods, logged what the DLP flagged and what it missed, and noted which bypass was easiest and why.
