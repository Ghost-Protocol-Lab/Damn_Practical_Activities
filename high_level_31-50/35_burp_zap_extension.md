# 35 — Write a Burp / ZAP Extension for a Recon Task

## What to Do
Automate a recon step you do manually during web testing by writing a custom extension for Burp Suite or OWASP ZAP — for example, auto-extracting interesting headers, flagging JWT tokens, or logging specific parameter patterns.

## Open Source Resources
- Burp Suite Extender API docs — portswigger.net/burp/extender
- ZAP Scripting documentation — zaproxy.org
- Example Burp extensions on GitHub (search "burp extension python")
- Jython (for Python-based Burp extensions)

## Tips
- Start with a passive scanner check, not an active one — it's simpler and less likely to cause unintended requests.
- Read three or four existing simple extensions before writing your own so you understand the boilerplate.
- Test it on a local DVWA or Juice Shop instance before pointing it at anything real.

## When It's Completed
The extension loads without errors, runs against a test target, and produces output that would have taken you manual effort to gather otherwise.
