# Pandesh v0.1.2 Alpha · Build 143 — UI fixes

**Status:** Fixes were implemented and acceptance was reported in the Windows development build. **This is not a public binary release yet.** The latest uploaded installer and portable ZIP are still [v0.1.1 Build 142](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha).

## What changed in Build 143

1. **New Conversation now starts clean.** The renderer was changed to prevent completed results, late model tokens and stale transcript refreshes from the previous conversation from appearing in a newly opened one.
2. **The top-right + New button works.** Both New buttons invoke the same conversation creation action instead of indirectly clicking another UI element.
3. **Tasks and Results are separate views.** Results are reachable in one click rather than appearing below a long list of tasks; outstanding approvals remain accessible.
4. **Product gallery refreshed.** [Six Build 143 screenshots](docs/SHOWCASE.md) show the updated application interface.

### Reported acceptance evidence

The development report records 5/5 targeted regression checks passing and packaged-app checks for the new-conversation reset and direct Results navigation. These are *reported development-build checks*, distinct from the previous Build 142 release acceptance. See the private development project's issue #75 for implementation context (requires source-repository access).

## Screenshots versus downloads

| Material | Version | Availability |
| --- | --- | --- |
| [Gallery](docs/SHOWCASE.md) | v0.1.2 · Build 143 | Public |
| [Current installer and portable ZIP](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha) | v0.1.1 · Build 142 | Public |
| v0.1.2 installer and portable ZIP | v0.1.2 · Build 143 | **Not uploaded to the public release** |

**Do not silently replace the v0.1.1 assets.** Publish a separate versioned release with matching source provenance, checksum sidecars and binaries only after verifying that the actual Build 143 artifacts exist and passed packaged acceptance. This ensures users downloading files see the behavior demonstrated in the updated screenshots.
