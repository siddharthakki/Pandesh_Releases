# Pandesh

**Pandesh** is a local-first AI assistant for Windows, powered by local AI models through [Ollama](https://ollama.com/).

> **Public alpha · v0.1.1 · Build 142**  
> This is early-access software. The first public release binaries are being transferred to this repository. **There is not yet a downloadable public release here.**

## Download

**[Open Pandesh Releases](https://github.com/siddharthakki/Pandesh_Releases/releases)**

When the `v0.1.1-pandesh-alpha` release is published here, download one of these Windows x64 packages:

| Package | When to use |
| --- | --- |
| `Pandesh-Setup.exe` | Standard per-user Windows installation |
| `Pandesh-v0.1.1-alpha-win32-x64-portable.zip` | Portable version; extract and run `Launch-Pandesh.cmd` |

**Do not download from unofficial mirrors.** Compare the downloaded file's SHA-256 with [SHA256SUMS.txt](SHA256SUMS.txt).

## Get started

1. Use Windows 10 or 11 (64-bit).
2. [Install Ollama](https://ollama.com/download) and start its local service.
3. Download an Ollama model suited to your hardware; for example, `ollama pull qwen2.5-coder:3b`. The release was also tested with `qwen3-coder:swift-27b` on higher-VRAM hardware.
4. Install Pandesh or extract the portable ZIP and run its launcher.
5. Select your available model in Pandesh, then start a conversation.

Example first questions: **“What can you do?”** and **“Run read-only system diagnostics.”**

## What the first alpha includes

- Local-model conversations with Ollama
- Governed execution of supported tasks and human approval for consequential actions
- Persistent memory, commitments, and task records
- Scheduled briefing and reminder infrastructure
- Read-only system diagnostics
- Process-management safety restrictions

## Validation and limitations

The private development project reports **27/27 Windows Sandbox acceptance checks passing** for clean install, process safety, shutdown, and data preservation, plus an isolated real-model workflow using `qwen3-coder:swift-27b`. These checks do not guarantee behavior on every Windows configuration.

**Known limitations:** This alpha is unsigned, so Windows SmartScreen may warn. Local Ollama must be installed and reachable; cloud fallback is disabled by default. Microphone functionality depends on your hardware and permissions. Some integrations require separate authorization.

You can verify the installer checksum using PowerShell:

```powershell
Get-FileHash .\Pandesh-Setup.exe -Algorithm SHA256
```

## Feedback

Use the [Issues](https://github.com/siddharthakki/Pandesh_Releases/issues) section to report installation, launch, model connectivity, or process-safety problems. Please include Pandesh version/build, Windows version, model and steps to reproduce. **Never post tokens, credentials, private emails, personal data, or unredacted logs.**

This repository is for **public release downloads and release support**. The development source repository is maintained separately.
