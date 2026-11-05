# Changelog

All changes to the project will be documented in this file.

- The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
- The date format is YYYY-MM-DD.
- The upcoming release version is named `vNext` and links to the changes between latest version tag and git HEAD.

## [vNext] - unreleased

- "It was a bright day in April, and the clocks were striking thirteen." - 1984

- Poll LunarG every 6 hours instead of running weekly on Sundays.
- Split the workflow into `check`, `build`, and `release` jobs.
- Only build when the LunarG version has no complete GitHub release yet.
- Download the version-specific LunarG tarball so the build matches the release tag.
- Create releases as drafts, upload all artifacts, and publish only when complete.
- Mark a release as latest only when it matches LunarG's current version.
- Rebuild and republish releases with missing assets.

- tag 1.4.313.0

<!-- Section for Reference Links -->

[vNext]: https://github.com/jakoch/vulkan-sdk-arm/compare/v0.0.1...HEAD
