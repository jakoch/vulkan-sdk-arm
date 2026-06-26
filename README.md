[![GitHub Releases](https://img.shields.io/github/release/jakoch/vulkan-sdk-arm.svg?style=flat-square)](https://github.com/jakoch/vulkan-sdk-arm/releases/latest)
[![GitHub Workflow Status](https://github.com/jakoch/vulkan-sdk-arm/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/jakoch/vulkan-sdk-arm/actions/workflows/build.yml)

# vulkan-sdk-arm

This repository contains a Github Action workflow, which builds the Vulkan SDK for ARM64 runners.

The SDK is build on the following runners:
- [ubuntu-22.04-arm](https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2204-Arm64-Readme.md)
- [ubuntu-24.04-arm](https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2404-Arm64-Readme.md)
- [ubuntu-26.04-arm](https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2604-Arm64-Readme.md)

The existing x86_64 binaries in the Vulkan SDK are replaced with aarch64 binaries.

The SDKs are automatically built and released whenever a new official Vulkan SDK is published.

The released packages are used by [jakoch/install-vulkan-sdk-action](https://github.com/jakoch/install-vulkan-sdk-action), enabling seamless integration into a GitHub Action workflow with the specified runners.

## Availability of Vulkan SDK ARM64 Prebuilt Binaries for Linux

Currently, KHRONOS has no plans to modify the official tarball to include prebuilt ARM binaries or to update the Ubuntu packages for ARM.

This repository automates the process by downloading the official Vulkan SDK tarball, building it for ARM, and repackaging the necessary binaries into the SDK.

## License

All the content in this repository is licensed under the MIT License.

Copyright (c) 2025 Jens A. Koch
