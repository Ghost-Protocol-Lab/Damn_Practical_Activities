# 11 — Establish an Email/Phishing Detection System and Try to Bypass It

## What to Do
Set up a free or open-source email security layer (e.g., a self-hosted mail server with SpamAssassin, or a cloud inbox's built-in phishing filters) and then attempt to craft messages that slip past it — entirely within accounts and infrastructure you own.

## Open Source Resources
- SpamAssassin
- Mail-in-a-Box (self-hosted mail server)
- GoPhish (for crafting test payloads)
- Google Workspace security sandbox settings (as a managed alternative)

## Tips
- Vary one evasion technique at a time (header spoofing, lookalike domains, URL obfuscation) so you can isolate which one actually worked.
- Test against the filter's default rules first before tuning anything.
- Keep every test message, sender, and recipient inside accounts you control.

## When It's Completed
You've logged which techniques were flagged versus which slipped through, and written up why the filter missed what it missed.
