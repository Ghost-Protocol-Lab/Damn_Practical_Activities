# 31 — Find a Vulnerability in an Open Source App

## What to Do
Pick a real open source application (a web app, CLI tool, or library with a public repo) and audit it manually for security flaws — logic bugs, injection points, broken auth, insecure defaults. If you find something real, report it responsibly.

## Open Source Resources
- GitHub (search for small-to-mid-size projects with no security policy yet)
- OWASP Testing Guide — owasp.org
- Semgrep (static analysis scanner to guide manual review)
- HackerOne's public disclosure reports for inspiration on bug classes

## Tips
- Smaller projects with fewer contributors are more likely to have overlooked bugs than major frameworks with dedicated security teams.
- Start with the most complex or user-facing logic — authentication, file upload, data parsing.
- Even a "won't fix" response from a maintainer counts if your report is technically sound.

## When It's Completed
You've audited the codebase, found at least one credible issue (even minor), and either submitted a responsible disclosure or documented why it was not reportable.
