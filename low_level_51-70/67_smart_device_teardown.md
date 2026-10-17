# 67 — Tear Down a Smart Device and Identify Its Communications Protocol

## What to Do
Physically disassemble a cheap smart device you own (a smart plug, IP camera, router, or OBD-II dongle) and identify its hardware components, debug interfaces (UART, JTAG), and wireless communications protocol (Zigbee, Z-Wave, BLE, Wi-Fi).

## Open Source Resources
- FCC ID database — fcc.gov/oet/ea/fccid (look up any device's internal photos pre-teardown)
- Saleae Logic Analyzer (or clone) for protocol analysis
- Wireshark BLE capture (with a compatible adapter)
- Zigbee2MQTT for Zigbee sniffing — zigbee2mqtt.io
- OpenWRT wiki (for router hardware identification)

## Tips
- Check the FCC ID before opening anything — the internal photos are often already public.
- Look for UART pads near the CPU and test them with a multimeter for 3.3V TX/RX signals — many devices have an open debug console accessible this way.
- Chip markings are your friend: search the IC part numbers to find datasheets and understand exactly what each chip does.

## When It's Completed
You've identified all major ICs, found at least one debug interface, and documented the device's communications protocol with a diagram of the hardware architecture.
