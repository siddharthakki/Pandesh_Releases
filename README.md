# Pandesh 🐼

### Your local-first AI assistant for Windows

**Chat with local AI. Run supported tasks. Keep control of consequential actions.**

Pandesh connects to locally running [Ollama](https://ollama.com/) models and brings conversations, approvals, memory, reminders and assistant workflows into a desktop interface. It's an **early public alpha**: try it, tell us what worked, and help us make the everyday experience reliable.

[**⬇ Download Pandesh for Windows (Build 143)**](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.2-pandesh-alpha) • [**📖 Getting started**](docs/GETTING_STARTED.md) • [**🔧 Troubleshooting**](docs/TROUBLESHOOTING.md) • [**🐞 Report an issue**](https://github.com/siddharthakki/Pandesh_Releases/issues) • [**📦 Source Code**](https://github.com/siddharthakki/Pandesh)

> **Current release:** v0.1.2 Public Alpha • Build 143 • Windows 10/11 x64  
> **Source code:** [github.com/siddharthakki/Pandesh](https://github.com/siddharthakki/Pandesh) (MIT License)

---

## Download

| Package | Link | Best for |
| --- | --- | --- |
| **Windows Installer** | [Download Pandesh-Setup.exe (Build 143)](https://github.com/siddharthakki/Pandesh_Releases/releases/download/v0.1.2-pandesh-alpha/Pandesh-Setup.exe) | Most Windows users |
| **Portable ZIP** | [Download portable version (Build 143)](https://github.com/siddharthakki/Pandesh_Releases/releases/download/v0.1.2-pandesh-alpha/Pandesh-v0.1.2-alpha-win32-x64-portable.zip) | Extract and launch without a standard install |
| **Checksums** | [SHA256SUMS.txt](SHA256SUMS.txt) | Verify downloads |

**Important:** The binaries are not code-signed yet. Download only from this official repository and check the checksum before running. This alpha requires a separate Ollama installation and at least one installed model.

## See Pandesh in action

**[Screenshots & walkthrough gallery ➔](docs/SHOWCASE.md)**

Tested from **the actual packaged alpha Build 143**.

| Experience | What is demonstrated |
| --- | --- |
| 🐼 **Chat** | First launch, conversation and the Panda interface |
| 🧠 **Local AI** | Selecting or connecting an installed Ollama model |
| 🔍 **Diagnostics** | A genuine read-only tool request and returned results |
| 🛡️ **Approvals** | Request ➔ review ➔ approval or rejection ➔ outcome |
| 📋 **Tasks & Results** | Dedicated Tasks and Results tabs with honest execution evidence |
| ⏰ **Daily assistant** | Reminders, memory and briefing workflow where configured |

## Quick start — 3 steps

**1. Install Ollama** from [ollama.com/download](https://ollama.com/download), then in PowerShell:

```powershell
ollama pull qwen2.5-coder:3b
ollama list
```

**2. [Download Pandesh Build 143](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.2-pandesh-alpha)** and install it (or extract the portable ZIP and run `Launch-Pandesh.cmd`).

**3. Launch Pandesh** and start with:

> Hi Pandesh — introduce yourself and tell me what you can do.

Then try a read-only request:

> Run read-only system diagnostics and show what you actually checked.

See the [complete step-by-step guide](docs/GETTING_STARTED.md) for model setup, permissions, memory, reminders and safety tips.

## What's included in Build 143?

- **Local-model chat** through Ollama
- **New Conversation navigation fix:** clean reset without stuck views
- **Tasks & Results views:** direct inspection of pending and completed outcomes
- **Installer isolation & safety:** upgraded installer cannot touch unrelated processes or data outside its directory
- **Governed actions:** user approval for consequential operations, with evidence-backed outcomes
- **Persistent memory, commitments and task records**
- **Scheduling** for assistant briefings and follow-ups
- **Read-only system diagnostics** and runtime health information

## Credits, third-party software and licenses

Pandesh builds on [Pi Agent Core / Pi AI](https://github.com/earendil-works/pi), [Electron](https://github.com/electron/electron), and other open-source libraries. It connects to separately installed tools such as [Ollama](https://ollama.com/), and supports optional integrations with [OpenCode](https://github.com/anomalyco/opencode) and [Hermes Agent](https://github.com/NousResearch/hermes-agent) when configured.

**[View third-party acknowledgements and license information](THIRD_PARTY_NOTICES.md).** Full Core source code is available at [github.com/siddharthakki/Pandesh](https://github.com/siddharthakki/Pandesh).

## Help shape Pandesh

We want real reports from people who actually install and use the assistant.

**[🐞 Report a bug or request a usability improvement](https://github.com/siddharthakki/Pandesh_Releases/issues)**

Helpful details: Pandesh version/build, Windows version, local model, a concise reproduction, and a **redacted** screenshot/video if relevant. **Do not post credentials, private emails, unredacted logs, or your Core data directory.**

---

[Releases](https://github.com/siddharthakki/Pandesh_Releases/releases) • [Getting started](docs/GETTING_STARTED.md) • [Troubleshooting](docs/TROUBLESHOOTING.md) • [Media showcase](docs/SHOWCASE.md) • [Checksums](SHA256SUMS.txt) • [Credits & licenses](THIRD_PARTY_NOTICES.md)