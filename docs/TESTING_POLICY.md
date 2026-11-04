# Testing policy

## Safe development boundary

Initial development and testing must stay within documented emulator workflows. This repository does not provide phone-flashing instructions, bootloader modification steps, partition-writing commands, or recovery procedures.

Do not:
- Unlock or modify a phone bootloader as part of following this repository.
- Write experimental images to boot, recovery, vendor, super, or other device partitions.
- Repartition, erase, or replace the Android installation.
- Use an unverified image on a personal or shared device.
- Disable platform security controls or bypass activation and signing protections.

## Emulator-first rule

Before any future hardware proposal, require:
- A reproducible source revision and build environment.
- A clear explanation of what the artifact is and what it is not.
- Successful tests in the intended, documented emulator.
- A review of legal, licensing, and safety implications.
- A separate, independently reviewed test plan for any supported development hardware.

## Artifact handling

Do not publish files named as bootable images unless they are actually generated, validated, and their purpose and limitations are clear. Never describe an untested build as bootable or safe to install.
