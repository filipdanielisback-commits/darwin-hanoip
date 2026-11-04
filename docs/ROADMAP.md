# Research roadmap

All milestones are exploratory. A milestone is complete only when its evidence and limitations are documented.

## Phase 0 — Project setup

- [x] Create repository and document scope.
- [x] Link the official XNU source.
- [ ] Record the selected upstream XNU tag and commit SHA.
- [ ] Add source references for the Moto G60 platform.

## Phase 1 — Emulator research

- [ ] Identify an officially documented emulator target supported by the selected XNU source.
- [ ] Set up a reproducible build environment using upstream documentation.
- [ ] Record required tools, SDKs, headers, and build limitations.
- [ ] Build only for the documented emulator target.
- [ ] Capture logs and record whether the result boots in that emulator.

## Phase 2 — Moto G60 platform study

- [ ] Confirm device codename, board identifiers, SoC, memory, storage, display, and peripherals from reliable sources.
- [ ] Locate and review public Android kernel and device-tree sources.
- [ ] Map which required hardware interfaces have public documentation.
- [ ] Document missing source, firmware, and driver dependencies.
- [ ] Assess boot-chain and platform compatibility at a high level without modifying a device.

## Phase 3 — Feasibility assessment

- [ ] Compare the upstream XNU platform assumptions with the documented Moto G60 hardware.
- [ ] Identify the minimum platform components that would be needed.
- [ ] Separate technically plausible work from unsupported assumptions.
- [ ] Publish a go/no-go report before any device-specific implementation is considered.

## Phase 4 — Compatibility research

Only proceed if the feasibility report identifies a lawful, technically credible path. Keep development in an emulator or other supported test environment. Do not create or distribute a phone installer or flashable image as part of this roadmap.

## Explicitly not promised

A bootable Moto G60 image, iOS 26 user space, Apple services, App Store, activation, cellular, camera, GPU acceleration, Wi-Fi, Bluetooth, touchscreen, or battery reporting. Each would require separate evidence and implementation.
