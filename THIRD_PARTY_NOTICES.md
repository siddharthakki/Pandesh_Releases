# Third-party software, acknowledgements and license information

**Pandesh v0.1.1 public alpha (Build 142)**

Pandesh is built using third-party open-source projects, frameworks, build tools, optional integrations and separately downloaded AI models. We acknowledge their authors and the upstream projects below.

**Important:** This page is a *verified, high-level attribution index*, **not yet the complete machine-generated license-notices inventory** of all bundled components and their transitive dependencies. Work to verify and include every applicable binary redistribution notice is tracked separately. Do not interpret a link or a high-level license label as a substitute for the license text required by a particular redistributed component.

## Pandesh's own source and release repository

- The Pandesh development project's `LICENSE` at the v0.1.1 alpha source release specifies **MIT**, copyright © 2026 Siddharth Akkinepalli. Its root `package.json` also declares `"license": "MIT"`.
- The [Pandesh_Releases `LICENSE`](LICENSE) is MIT. It governs material to which that license is applicable in this public repository; it does not override upstream licenses of included third-party software, externally installed programs, images, trademarks or separately obtained AI model weights.
- The development repository is private at this release. The release binaries are available [here](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha).
- License and attribution declarations must remain consistent with the actual release package. **A private repository is not automatically proprietary, and a public download is not automatically a source-code release.**

## Runtime and packaged frameworks

The pinned alpha source declares the following direct dependencies. Some are bundled into the desktop application; the packaging-specific inventory still requires verification.

| Project | Pandesh relationship | Upstream source and license reference |
| --- | --- | --- |
| **Pi Agent Core** (`@earendil-works/pi-agent-core`) | Direct runtime dependency and agent execution support; alpha accepted with v1.2.0 | [Pi by Earendil Works](https://github.com/earendil-works/pi) · [MIT license](https://github.com/earendil-works/pi/blob/main/LICENSE) |
| **Pi AI** (`@earendil-works/pi-ai`) | Direct runtime dependency for model/provider integration; alpha accepted with v1.2.0 | [Pi by Earendil Works](https://github.com/earendil-works/pi) · [MIT license](https://github.com/earendil-works/pi/blob/main/LICENSE) |
| **Electron** (33.4.11) | Packaged Windows desktop shell | [Electron](https://github.com/electron/electron) · [MIT license](https://github.com/electron/electron/blob/main/LICENSE) |
| **React** and **React DOM** | Declared UI dependencies | [React](https://github.com/facebook/react) · [MIT license](https://github.com/facebook/react/blob/main/LICENSE) |
| **Shiki**, **Streamdown**, **TypeBox**, **Undici** and **@vscode/sqlite3** | Declared application dependencies; precise shipped versions are determined by lockfile/build | [Shiki](https://github.com/shikijs/shiki), [Streamdown](https://github.com/vercel/streamdown), [TypeBox](https://github.com/sinclairzx81/typebox), [Undici](https://github.com/nodejs/undici), [VS Code SQLite3](https://github.com/microsoft/vscode-sqlite3) — review the license in the exact locked package |
| **Chromium, Node.js and associated native components** | Included through Electron/desktop runtime | Their bundled third-party notices and licenses must be preserved; see Electron and the installed runtime's notices |

Package names and dependency listings do **not** establish that the release bundles every declared dependency. Conversely, components bundled transitively may not be listed here.

## Separately installed integrations and services

These products are **not claimed to be bundled in the Pandesh installer**. They are supported or referenced through runtime adapters and may require installation, configuration or authentication by the user.

| Project/service | Relationship | Official source or terms |
| --- | --- | --- |
| **Ollama** | Local model server for the first alpha; users install it separately | [Ollama](https://ollama.com/) · [GitHub / MIT](https://github.com/ollama/ollama) |
| **OpenCode** | Optional separately installed coding-engine CLI/server invoked by a Pandesh adapter | [OpenCode](https://github.com/anomalyco/opencode) · [MIT license](https://github.com/anomalyco/opencode/blob/dev/LICENSE) |
| **Hermes Agent** (Nous Research) | Optional separately running agent service/skills integration; not required for basic Pandesh chat | [Hermes Agent](https://github.com/NousResearch/hermes-agent) · [MIT license](https://github.com/NousResearch/hermes-agent/blob/main/LICENSE) |
| **Google Gmail and Calendar** | Optional connected services requiring explicit Google authorization | [Google API Terms](https://developers.google.com/terms) |
| **OpenRouter** | Optional provider integration where configured by the user | [OpenRouter](https://openrouter.ai/) · [Terms](https://openrouter.ai/terms) |

A project being mentioned here does **not** imply sponsorship, endorsement, partnership, or that it is installed or active for every user. Third-party brand names and trademarks remain the property of their respective owners.

## Build and installation tools

**Inno Setup 6.7.3** is used to create the Windows installer. The project has its **own Inno Setup License**, which should not be described simply as MIT. See [official license text](https://github.com/jrsoftware/issrc/blob/main/license.txt) and [Inno Setup website](https://jrsoftware.org/). The project requests commercial users purchase a license; consult the [official licensing information](https://jrsoftware.org/isorder.php) for applicability. <https://spdx.org/licenses/InnoSetup.html>

Development/testing tools such as TypeScript, esbuild, Vitest and other npm packages have their own licenses. A final complete list should be produced from the actual lockfile **and packaged files**.

## AI models and generated content

Pandesh is an application, **not a provider or licensor of the user's local AI models**. Model names (such as Qwen or GPT-OSS) identify third-party models installed independently through Ollama or another provider. **Each model's weights, outputs and usage restrictions are governed by its own applicable model license and provider terms**, which may differ from both MIT and Ollama's software license. Users should review these terms before redistribution or commercial use.

## Required complete redistribution-notices audit

Before describing the distribution as having *complete* third-party notices, the maintainer should:

1. Inventory the **exact** production components in `Pandesh-Setup.exe` and the portable ZIP, including all dependencies bundled into Electron/Node.js/Chromium and any native binary resources.
2. Match each artifact and version to its copyright owners, license identifiers and **full required notice/license text** (not merely links). Retain any upstream `LICENSE`, `NOTICE`, and attribution obligations.
3. Cross-check the lockfile, Electron's packaged notice files, installer payload, embedded fonts/icons/images and any shipped third-party assets. Check copyleft obligations and permissions for any assets that are not under a permissive code license.
4. Generate a versioned `THIRD_PARTY_LICENSES` / `NOTICE` distribution artifact, include it with the release and where necessary inside the installed application, and add a repeatable check to the packaging pipeline.
5. Review this page and regenerate the notices whenever dependencies, bundled assets or build tooling change.

If a missing attribution or potential license issue is found, please [file a release issue](https://github.com/siddharthakki/Pandesh_Releases/issues) with the component name, version and upstream license source.

---

This page documents observed project dependencies and official upstream sources. It is not legal advice or a warranty of full license compliance. For a component's legally controlling terms, consult the exact license supplied with its redistributed version.
