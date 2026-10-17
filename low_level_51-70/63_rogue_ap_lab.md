# 63 — Set Up a Rogue Access Point in a Lab and See What Auto-Connects

## What to Do
In a controlled lab environment using hardware you own, broadcast a Wi-Fi SSID that mimics a common network name (e.g., "xfinitywifi", "Starbucks") and observe which of your own devices auto-connect — demonstrating the evil twin / karma attack concept.

## Open Source Resources
- hostapd (Linux AP daemon) — w1.fi/hostapd
- airbase-ng (part of Aircrack-ng suite)
- Bettercap — bettercap.org
- Kali Linux (has all tools pre-installed)

## Tips
- Only test with your own devices on your own network — broadcasting on shared spectrum requires care about who else might connect.
- Watch what traffic the connecting device sends immediately after association — devices often phone home instantly.
- This demonstrates why "auto-connect to known networks" is dangerous and why SSID alone is not an authenticator.

## When It's Completed
At least one of your own devices auto-connected, you've captured its first-burst traffic, and you can explain what a real attacker would do with that position.
