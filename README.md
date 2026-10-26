# Pandesh 🐼 — Windows Personal AI Assistant

**Local AI conversations, governed execution, approvals and everyday desktop assistant workflows for Windows.**

Looking for an Ollama desktop companion, an open-source personal AI assistant for Windows, or an alternative to cloud-only assistants? Pandesh runs local LLMs on your computer and combines conversations, memory, scheduled briefings and human approvals in an approachable Panda interface.

[**⬇ Download Pandesh Build 145**](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.4-pandesh-alpha) • [**📖 Getting started**](docs/GETTING_STARTED.md) • [**🔧 Troubleshooting**](docs/TROUBLESHOOTING.md) • [**🐞 Report an issue**](https://github.com/siddharthakki/Pandesh_Releases/issues) • [**📦 Source Code**](https://github.com/siddharthakki/Pandesh)

> **Current release:** v0.1.4 Public Alpha (Build 145) • Windows 10/11 x64  
> **Source code:** [github.com/siddharthakki/Pandesh](https://github.com/siddharthakki/Pandesh) (MIT License)

---

## Download

| Package | Link | Best for |
| --- | --- | --- |
| **Windows Installer** | [Download Pandesh-Setup.exe (Build 145)](https://github.com/siddharthakki/Pandesh_Releases/releases/download/v0.1.4-pandesh-alpha/Pandesh-Setup.exe) | Most Windows users |
| **Portable ZIP** | [Download portable version (Build 145)](https://github.com/siddharthakki/Pandesh_Releases/releases/download/v0.1.4-pandesh-alpha/Pandesh-v0.1.4-alpha-win32-x64-portable.zip) | Extract and launch without a standard install |
| **Checksums** | [SHA256SUMS.txt](SHA256SUMS.txt) | Verify downloads |

**This alpha is unsigned.** Install from the official GitHub release only, verify the checksum, and carefully review any Windows warning.

## Set up in three steps

1. Install [Ollama for Windows](https://ollama.com/download).
2. In PowerShell, install a model: `ollama pull qwen2.5-coder:3b`. Confirm `ollama list` shows it.
3. Install Pandesh Build 145 (or extract the entire portable ZIP and launch `Launch-Pandesh.cmd`), then start a conversation.

See the [full setup guide](docs/GETTING_STARTED.md) and [troubleshooting FAQ](docs/TROUBLESHOOTING.md).

## What can Pandesh do?

- Run supported local AI model conversations through Ollama
- Record governed memory and tasks, with permissioned execution and observable outcomes
- Direct Tasks and Results views with honest execution evidence
- Offer daily assistant workflows, reminders and follow-ups where scheduling and connectors are configured
- Provide read-only diagnostics and results presentation when supported
- Work with optional external tools/providers when separately installed or authorized

**Alpha reality:** model compatibility varies; model self-identification, permission-aware follow-ups and some UI behaviors are still being improved. A model claiming a tool ran does not prove it did. An external connector with insufficient permissions cannot complete that task.

## Screenshots and demos

[**See the full six-image gallery →**](docs/SHOWCASE.md)

[![Pandesh Tasks and Results Build 145](assets/screenshots/06-completed-tasks-and-results.png)](docs/SHOWCASE.md)

These screenshots show the **updated Build 145 desktop application** with New Conversation and Results navigation fixes.

## Help test and improve Pandesh

Your real Windows/Ollama experience is valuable—even if you're not a developer.

**[Report a bug or model compatibility result](https://github.com/siddharthakki/Pandesh_Releases/issues/new/choose)** · **[Start contributing](https://github.com/siddharthakki/Pandesh/blob/main/docs/CONTRIBUTOR_START_HERE.md)** · **[Good first issues](https://github.com/siddharthakki/Pandesh/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)**

Please include your installed build and steps that demonstrate what actually worked. Never post credentials, private data or unredacted logs.

## Project and roadmap

- [**Open-source project**](https://github.com/siddharthakki/Pandesh) — MIT license, public architecture, contribution/security policies
- [**Architecture diagram**](https://github.com/siddharthakki/Pandesh/blob/main/docs/ARCHITECTURE.md) — desktop, Core, models, external integrations and approval lifecycle
- [**Roadmap**](https://github.com/siddharthakki/Pandesh/blob/main/docs/ROADMAP.md) — real-world reliability before feature expansion
- [**Privacy and safety**](https://github.com/siddharthakki/Pandesh/blob/main/docs/PRIVACY.md)
- [**Third-party acknowledgements**](THIRD_PARTY_NOTICES.md)

## Tested release baseline

The development report records **27/27 isolated Windows Sandbox checks** for the release candidate and a local model acceptance journey using `qwen3-coder:swift-27b`. These reported results do not guarantee every model, tool or Windows configuration.

[Release notes](RELEASE_NOTES.md) · [Checksums](SHA256SUMS.txt) · [Report a bug](https://github.com/siddharthakki/Pandesh_Releases/issues)

---

*Pandesh is an independent project. “Jarvis-style” describes the personal-assistant concept; it does not imply affiliation with Marvel/J.A.R.V.I.S. or other products. Third-party software, services and AI model weights retain their own licenses.*