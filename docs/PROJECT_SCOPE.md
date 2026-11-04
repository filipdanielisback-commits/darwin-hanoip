# Project scope

## What this project is

`darwin-hanoip` is an educational investigation into XNU/Darwin and the publicly documented Motorola Moto G60 platform. The long-term question is whether any meaningful compatibility work is technically possible.

The intended direction is real kernel and operating-system research, not an Android launcher, skin, or imitation interface.

## In scope

- Read and document Apple's publicly released XNU source.
- Track upstream source versions and their licenses.
- Study public Moto G60 kernel/device-tree sources and hardware documentation.
- Identify differences between generic ARM64 support and actual board support.
- Create reproducible build notes for supported emulator targets.
- Record unknowns, blockers, and test evidence honestly.

## Out of scope

- Claiming that an unmodified iOS 26 image can boot on the Moto G60.
- Redistributing Apple's proprietary iOS user space, firmware, keys, or signing materials.
- Bypassing activation, Apple ID, DRM, secure boot, or other security controls.
- Publishing instructions or scripts that overwrite phone partitions.
- Promising App Store, Apple services, cellular, camera, GPU, Wi-Fi, Bluetooth, or touchscreen support without verified implementation and testing.

## Evidence standard

Every hardware-support claim must link to its source and state whether it is merely researched, compiled, emulator-tested, or tested on supported hardware. Unknown means unknown; do not mark a feature as working based on a similar chipset or another phone's port.
