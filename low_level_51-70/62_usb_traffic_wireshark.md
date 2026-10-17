# 62 — Analyze a USB Device's Traffic with Wireshark's USBPcap

## What to Do
Capture USB traffic between your computer and a device you own (keyboard, mouse, USB storage, or Arduino) using USBPcap and Wireshark, then decode the protocol and understand what data is being transferred.

## Open Source Resources
- USBPcap — desowin.org/usbpcap (Windows USB capture driver)
- Wireshark USB dissectors — built-in
- Linux usbmon (built-in USB capture for Linux — no extra install)
- USB HID protocol specification (for keyboard/mouse decoding)

## Tips
- On Linux, `modprobe usbmon` and then capture on the usbmon interface directly in Wireshark — no extra tools needed.
- A USB keyboard is the most educational target: you can decode actual keystrokes from the HID packets.
- Filter by `usb.transfer_type == 0x01` (interrupt transfers) to isolate HID device communications.

## When It's Completed
You've captured USB traffic from a device, decoded at least one meaningful transaction (a keystroke, a file read, a command), and can explain the structure of the USB packets involved.
