# Pandesh 🐼 — Download the Local AI Personal Assistant for Windows

**A Jarvis-style personal AI assistant that runs local AI models through Ollama and helps with real tasks under your control.**

Pandesh is a **Windows desktop AI assistant** designed for local LLM conversations, governed task execution, reminders, memory and practical day-to-day workflows. If you're exploring **self-hosted AI assistants**, **Ollama tools**, or a personal assistant you can run on your own PC, start here.

[**⬇ Get Pandesh v0.1.1 Alpha**](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha) · [**📖 Setup guide**](docs/GETTING_STARTED.md) · [**🖼 Screenshots**](docs/SHOWCASE.md) · [**🏗 Architecture**](https://github.com/siddharthakki/Pandesh/blob/main/docs/ARCHITECTURE.md) · [**🐛 Feedback**](https://github.com/siddharthakki/Pandesh_Releases/issues)

![Pandesh v0.1.2 Build 143 updated Panda desktop interface](assets/screenshots/01-welcome-chat.png)

<sub>The screenshots show the **fixed v0.1.2 Build 143** interface. The current public installer is still **v0.1.1 Build 142** until the newer binaries are published. See the [Build 143 fixes](BUILD_143_FIXES.md).</sub>

## Download for Windows

| Package | Direct download | When to choose |
| --- | --- | --- |
| **Windows installer** | [Pandesh-Setup.exe](https://github.com/siddharthakki/Pandesh_Releases/releases/download/v0.1.1-pandesh-alpha/Pandesh-Setup.exe) | Recommended Windows 10/11 x64 installation |
| **Portable ZIP** | [Pandesh-v0.1.1-alpha-win32-x64-portable.zip](https://github.com/siddharthakki/Pandesh_Releases/releases/download/v0.1.1-pandesh-alpha/Pandesh-v0.1.1-alpha-win32-x64-portable.zip) | Extract and launch without a standard installation |
| **SHA-256** | [SHA256SUMS.txt](SHA256SUMS.txt) | Check downloaded files against the expected hashes |

**This alpha is unsigned.** Install from the official GitHub release only, verify the checksum, and carefully review any Windows warning.

## Set up in three steps

1. Install [Ollama for Windows](https://ollama.com/download).
2. In PowerShell, install a model: `ollama pull qwen2.5-coder:3b`. Confirm `ollama list` shows it.
3. Install Pandesh (or extract the entire portable ZIP and launch `Launch-Pandesh.cmd`), then start a conversation.

See the [full setup guide](docs/GETTING_STARTED.md) and [troubleshooting FAQ](docs/TROUBLESHOOTING.md).

## What can Pandesh do?

- Run supported local AI model conversations through Ollama
- Record governed memory and tasks, with permissioned execution and observable outcomes
- Offer daily assistant workflows, reminders and follow-ups where scheduling and connectors are configured
- Provide read-only diagnostics and results presentation when supported
- Work with optional external tools/providers when separately installed or authorized

**Alpha reality:** model compatibility varies; model self-identification, permission-aware follow-ups and some UI behaviors are still being improved. A model claiming a tool ran does not prove it did. An external connector with insufficient permissions cannot complete that task.

## Screenshots and demos

[**See the full six-image gallery →**](docs/SHOWCASE.md)

[![Pandesh Tasks and Results development preview](assets/screenshots/06-completed-tasks-and-results.png)](docs/SHOWCASE.md)

These screenshots show the **updated Build 143 desktop application** with New Conversation and Results navigation fixes. They are ahead of the currently published Build 142 installer; the patch release is not yet uploaded. **No walkthrough MP4 is attached yet.**

## Help test and improve Pandesh

Your real Windows/Ollama experience is valuable—even if you're not a developer.

**[Report a bug or model compatibility result](https://github.com/siddharthakki/Pandesh_Releases/issues/new/choose)** · **[Start contributing](https://github.com/siddharthakki/Pandesh/blob/main/docs/CONTRIBUTOR_START_HERE.md)** · **[Good first issues](https://github.com/siddharthakki/Pandesh/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)**

Please include your installed build and steps that demonstrate what actually worked. Never post credentials, private data or unredacted logs.

## Project and roadmap

- [**Open-source project**](https://github.com/siddharthakki/Pandesh) — MIT license, public architecture, contribution/security policies, source publication gates
- [**Architecture diagram**](https://github.com/siddharthakki/Pandesh/blob/main/docs/ARCHITECTURE.md) — desktop, Core, models, external integrations and approval lifecycle
- [**Roadmap**](https://github.com/siddharthakki/Pandesh/blob/main/docs/ROADMAP.md) — real-world reliability before feature expansion
- [**Privacy and safety**](https://github.com/siddharthakki/Pandesh/blob/main/docs/PRIVACY.md)
- [**Third-party acknowledgements**](THIRD_PARTY_NOTICES.md)

**Source publication is in preparation.** The new MIT source repository does not yet contain the complete reviewed Core; development history remains private until the security and redistribution checks are complete.

## Tested release baseline

The development report records **27/27 isolated Windows Sandbox checks** for the release candidate and a local model acceptance journey using `qwen3-coder:swift-27b`. These reported results do not guarantee every model, tool or Windows configuration.

[Release notes](RELEASE_NOTES.md) · [Checksums](SHA256SUMS.txt) · [Report a bug](https://github.com/siddharthakki/Pandesh_Releases/issues)

---

*Pandesh is an independent project. “Jarvis-style” describes the personal-assistant concept; it does not imply affiliation with Marvel/J.A.R.V.I.S. or other products. Third-party software, services and AI model weights retain their own licenses.*
