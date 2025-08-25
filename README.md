# Native Binaryen Libraries CI

This repository contains a GitHub Actions workflow to build and publish native shared libraries and CLI tools for [Binaryen](https://github.com/WebAssembly/binaryen) across major platforms.

## What This Repo Does
- Builds Binaryen native shared libraries and CLI tools for:
  - Linux x64, Linux arm64
  - macOS ARM64, macOS x64
  - Windows x64
- Publishes artifacts as draft GitHub Releases for downstream CI and package managers.
- Includes upstream Binaryen license and commit metadata in each release.

## Usage
This repository is intended for maintainers or CI systems that need prebuilt Binaryen binaries for multiple platforms. To trigger a build:
1. Go to the **Actions** tab.
2. Select the **Build Native Libraries** workflow.
3. Click **Run workflow** and specify the Binaryen tag or commit (e.g., `version_116` or `main`).

Artifacts will be published as a draft release with platform-specific archives and a combined archive.


## Licensing
- The workflow code in this repository is released to the public domain under [The Unlicense](./UNLICENSE).
- **The binaries and LICENSE-BINARYEN files produced by the workflow are subject to the [Apache 2.0 license](https://github.com/WebAssembly/binaryen/blob/main/LICENSE) of the Binaryen project.**
- Each release includes the upstream Binaryen license and commit metadata.

## Disclaimer
This repository is not affiliated with the Binaryen project. It only automates building and publishing their official releases for convenience.

## See Also
- [Binaryen GitHub](https://github.com/WebAssembly/binaryen)
- [The Unlicense](https://unlicense.org/)

---

For questions or issues, please open an issue in this repository.
