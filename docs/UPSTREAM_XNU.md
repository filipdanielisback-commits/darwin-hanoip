# Upstream XNU source

## Official source locations

- Repository: https://github.com/apple-oss-distributions/xnu
- Apple Open Source releases: https://opensource.apple.com/releases/

Use Apple's official release pages and repository tags to select a source snapshot. Record the exact tag or commit SHA in research notes before attempting a build.

## iOS 26 version family

Public kernel build metadata for the original iOS 26.0 release identifies the kernel version as `25.0.0` and the build identifier as `12377.2.8~1`. This places it in the `xnu-12377` source-version family.

Important distinctions:

- `xnu-12377` is a source-version family, not a complete iOS 26 source release.
- A kernel build identifier such as `12377.2.8~1` is not necessarily the exact Git tag name.
- Later iOS 26 updates can use different kernel build identifiers and source snapshots.
- Do not assume the newest public XNU tag is a drop-in match for every iOS 26 device build.

Before selecting a baseline, record:
1. iOS release and build number being researched.
2. Corresponding kernel version/build identifier, with a source reference.
3. Exact Apple XNU tag or commit selected.
4. Relevant license and notice files.
5. Known differences between the public source snapshot and the target build.

## What Apple publishes—and what it does not

The public XNU repository is kernel source. It is not the complete iOS operating system. It does not provide all iOS applications and frameworks, all device-specific drivers, firmware, private SDKs, signing infrastructure, or every platform component.

An ARM64 code path in XNU does not establish support for a Qualcomm-based Motorola phone. Device-specific platform code and drivers are a separate, substantial research problem.

## Repository policy

This project links to Apple's upstream repository rather than vendoring a second copy. Do not add proprietary Apple system images, firmware, signing keys, or other restricted materials here. Preserve upstream copyright and license notices for any source excerpts that are legally appropriate to include.
