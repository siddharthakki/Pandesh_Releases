# Pandesh release security policy

This repository distributes public Windows alpha installers, portable packages and their accompanying checksums. **No untrusted contribution may directly create, replace or publish official binaries.**

## Report an issue

- **Installation, download, model compatibility or usability bug:** [File a public issue](https://github.com/siddharthakki/Pandesh_Releases/issues/new/choose) with a redacted reproducer.
- **Security issue:** report privately via **[Security → Advisories → Report a vulnerability](https://github.com/siddharthakki/Pandesh_Releases/security/advisories/new)**. Private vulnerability reporting is active. Do not post exploit details, credentials or private data in public issues.

## Official release integrity

- Source development and release packaging are tracked separately in [Pandesh](https://github.com/siddharthakki/Pandesh).
- All official installers must be tested on isolated Windows machines and versioned. Do not silently replace previously published binaries.
- Verify both artifact sizes and SHA-256 digests before publishing; publish checksums alongside packages.
- Checksums detect accidental or malicious file mismatch relative to published metadata, but **are not** a code signature, malware-scan result or proof that a build is safe.
- Release publishing tokens must not be shared with PR builds or contributors.
- No GitHub Actions PR workflow, runner or automated binary publication is configured here as of 2026-10-24.
- Do not run unknown executable attachments, suggested commands, or fork scripts on your own computer.

## Contribution boundaries

Anyone may suggest fixes, translations or documentation improvements in issues and PRs. Proposed files are **untrusted** until independently reviewed. Only maintainer-approved changes belong in the official docs; binary publishing requires a separate, verified maintainer operation.

The `.github/CODEOWNERS` file routes changes to the maintainer. An active branch ruleset protects `main`. See [maintainer security setup](https://github.com/siddharthakki/Pandesh/blob/main/docs/MAINTAINER_SECURITY_SETUP.md).

## Current release

The current public installer is **v0.1.1 Build 142**. Updated Build 143 screenshots show a newer development version that has not yet been published as a matching installer.

This project is an early alpha and cannot promise immunity from all malware, mistakes or security vulnerabilities.
