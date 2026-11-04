# Moto G60 (hanoip) research checklist

This document is a checklist, not a device-modification guide.

## Identity and sources

- [ ] Confirm exact model variant and regional SKU.
- [ ] Confirm codename and board/platform identifiers from multiple reliable sources.
- [ ] Link official or otherwise reputable kernel source.
- [ ] Link device-tree source and record its exact revision.
- [ ] Record Android kernel version and configuration where publicly available.

## Hardware inventory

For each item, record the evidence source and confidence level.

| Area | Information to verify | Status |
|---|---|---|
| SoC | Exact SoC and revision | Unknown |
| CPU | ARM architecture and core configuration | Unknown |
| Memory | RAM layout and reserved regions | Unknown |
| Storage | Controller and partition map documentation | Unknown |
| Boot | Publicly documented boot architecture | Unknown |
| Display | Panel, display controller, modes | Unknown |
| Touch | Touch controller and interface | Unknown |
| GPU | GPU model and available public documentation | Unknown |
| Wi-Fi/Bluetooth | Chipset, firmware dependencies, interfaces | Unknown |
| Audio | Codec and audio routing | Unknown |
| Camera | Sensors and ISP dependencies | Unknown |
| Power | Battery gauge, charging, thermal interfaces | Unknown |
| Sensors | Sensor hub and individual devices | Unknown |

## Compatibility questions

- Which XNU architecture and platform code is relevant?
- Are required platform interfaces publicly documented?
- Are essential drivers available under compatible licenses?
- Are required firmware components redistributable and legally usable?
- Is there a supported emulator or development platform for validating work?

A shared SoC with another phone does not mean the phones share board wiring, device trees, firmware, boot integration, or working drivers.

## Evidence labels

Use only these labels in future status reports:

- **Unknown** — not investigated or no reliable source found.
- **Documented** — supported by a cited public source.
- **Built** — compiled, with exact source revision and build logs recorded.
- **Emulator-tested** — exercised in a named emulator and configuration.
- **Hardware-tested** — tested on a supported development platform with a documented, safe procedure and evidence.

Do not label a Moto G60 feature “working” based solely on another device's results.
