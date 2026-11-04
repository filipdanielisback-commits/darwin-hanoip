# darwin-hanoip

**Experimental XNU/Darwin research for the Motorola Moto G60 (hanoip), investigating whether any iOS 26-era components can be studied or adapted.**

> **Status: research scaffold only.** This repository does not currently contain a working kernel, bootloader, iOS system image, device drivers, or a bootable `.img`. Nothing here is ready to install on a phone.

## Project goal

Study the public XNU source and the Moto G60's publicly documented hardware/software interfaces. Establish what can be built and tested safely in an emulator before making any claims about device support.

This is intended to be a genuine kernel/OS research project—not an Android launcher or an iOS-style theme.

## Important facts

- XNU is the kernel used by Apple's operating systems; it is not the whole iOS operating system.
- iOS 26 kernel build metadata uses the `12377` version family. That is a version-family identifier, not a promise that one public source tag exactly reproduces every iOS 26 build.
- Apple's public XNU repository contains published kernel source snapshots. It does **not** contain the complete iOS user space, all device firmware, every driver, Apple's signing infrastructure, or the complete iOS SDK.
- A kernel that builds for ARM64 is not automatically compatible with the Moto G60. Board support, boot integration, memory layout, interrupt controllers, storage, display, touch, networking, power management, and many other details would need independent investigation.

## Upstream source

- [Apple XNU source](https://github.com/apple-oss-distributions/xnu)
- [Apple Open Source releases](https://opensource.apple.com/releases/)
- [XNU version-family reference](docs/UPSTREAM_XNU.md)

We link to upstream source instead of copying Apple's source tree into this repository. Follow the upstream license and notices when using it.

## Repository guide

- [Project scope and non-goals](docs/PROJECT_SCOPE.md)
- [Research roadmap](docs/ROADMAP.md)
- [Device research checklist](docs/DEVICE_RESEARCH.md)
- [Safe testing policy](docs/TESTING_POLICY.md)
- [Current status](docs/STATUS.md)
- [Contributing](CONTRIBUTING.md)

## Current status

The repository is documentation and planning only. The first technical milestone is to establish a reproducible, emulator-only XNU research environment. No Moto G60 boot image or installer is provided.

## Safety and legal boundaries

- Do not use this repository as instructions to unlock, flash, repartition, or modify a phone.
- Do not overwrite Android boot, recovery, or other device partitions.
- Do not upload proprietary iOS system files, firmware, signing materials, or personal data.
- Do not attempt to bypass activation, Apple ID, DRM, secure boot, or other platform protections.
- Keep experiments in an emulator or other explicitly supported development environment until qualified device-specific research establishes a safe test plan.

## Disclaimer

This is an independent educational research project and is not affiliated with or endorsed by Apple or Motorola. “iOS 26 compatibility” is an investigation target, not a claim of compatibility or a promise that iOS 26, App Store apps, Apple services, or phone hardware will work.
