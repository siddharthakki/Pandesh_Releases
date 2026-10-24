# Pandesh — Getting Started

A practical walkthrough for **Pandesh v0.1.1 Public Alpha (Build 142)** on Windows 10/11 (64-bit).

[← Back to the download page](../README.md) · [Latest release](https://github.com/siddharthakki/Pandesh_Releases/releases/latest) · [Troubleshooting](TROUBLESHOOTING.md)

## 1. Download and verify Pandesh

Download from the [official Pandesh v0.1.1 alpha release](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha).

Choose one:

- **Pandesh-Setup.exe** — the normal Windows installer (recommended).
- **Pandesh-v0.1.1-alpha-win32-x64-portable.zip** — extract and start using `Launch-Pandesh.cmd`.

Optional but recommended: in PowerShell, from your Downloads folder, check the installer:

```powershell
Get-FileHash .\Pandesh-Setup.exe -Algorithm SHA256
```

Expected SHA-256:

```text
90BC64B793E60F376B8211FA28838049B789E216A67BC78BBCDDE243DC89557C
```

See [all checksums](../SHA256SUMS.txt). **Do not run a file whose checksum is different.** This is an unsigned alpha, so Windows may warn that the publisher is unknown. Only choose to run the software if you trust the official GitHub release and have verified the hash.

## 2. Install and start Ollama

Pandesh relies on a local AI model server. The first alpha was tested using **Ollama**.

1. Install Ollama from [ollama.com/download](https://ollama.com/download).
2. Launch the Ollama Windows application; it usually provides the local service.
3. Open PowerShell and download a starter model:

```powershell
ollama pull qwen2.5-coder:3b
ollama list
```

This example model is about 1.9 GB to download; it is a smaller model for trying Pandesh. Larger models may improve responses and tool use but demand more memory. The alpha's live acceptance was carried out with `qwen3-coder:swift-27b` on a powerful local PC, **not** with every model.

To check that Ollama's local API responds, run:

```powershell
Invoke-RestMethod http://127.0.0.1:11434/api/tags
```

If that command fails, check whether the Ollama application is running. See [troubleshooting](TROUBLESHOOTING.md).

## 3. Start Pandesh

**Installer:** Run `Pandesh-Setup.exe`, then open Pandesh from the Start menu or desktop shortcut.

**Portable:** Extract the entire ZIP to a dedicated folder, then run `Launch-Pandesh.cmd`. Do not run it directly inside the ZIP.

The first launch should connect to the local Pandesh Core. If no AI models appear, confirm Ollama is running and that `ollama list` displays a model. Use the model/provider settings if visible in your build.

## 4. Your first conversation

Start simple. Type one of these in Pandesh's chat composer:

> Hi Pandesh. Introduce yourself briefly.

> Explain what you can help me do in this version.

> Summarize our conversation in three sentences.

These should demonstrate basic model connectivity. If Pandesh replies that it cannot access a tool you expected, **do not assume the action happened**. Some tools are still being refined in this alpha.

## 5. Try an actual tool-assisted task

Try a low-risk, read-only request:

> Run read-only system diagnostics and tell me which local AI providers are reachable.

Supported tool availability depends on your Core and provider configuration. A successful run should show an actual result or tool evidence, not instructions for you to manually run commands.

If it merely says “I can't access your PC,” please [report the issue](https://github.com/siddharthakki/Pandesh_Releases/issues). Include the exact request, selected model, and whether Ollama was reachable. **Do not include tokens or private diagnostic values.**

## 6. Memory, approvals, and reminders

Example prompts:

> Remember that I prefer concise answers.

> Remind me tomorrow at 9:00 to review my notes.

> What's on my schedule today?

The application may request approval before remembering information or performing consequential actions. Review the action and destination carefully. Choose **Approve** only when the described action matches your request; otherwise reject it.

**A model saying “done” isn't proof of execution.** Look for a completed task, stored reminder, or other observable result. Calendar, Gmail and similar integrations require their own connections/permissions.

## 7. Briefings and integrations

Pandesh supports scheduled assistant routines. A daily briefing can draw from sources such as connected calendars and email, **only where you have authorized access**. Schedules, connectivity, source coverage, and model behavior vary. Check the actual next-run time and which services are connected.

Permission-denied results mean no access was granted; they are not successful mailbox or calendar operations.

## 8. Safety and privacy

- The local model runs via your local Ollama service; separate connected services may exchange data under their permissions.
- Review consequential actions, especially file operations and any system-management requests.
- Never publish Core tokens, raw logs, private emails, mailbox contents, or personal details in GitHub Issues.
- This is an **alpha**, not a guarantee of safe unattended behavior on every PC. Keep backups of important data.

## 9. Get help

- [Troubleshooting and FAQ](TROUBLESHOOTING.md)
- [Screenshots and demo video](SHOWCASE.md)
- [Report a problem](https://github.com/siddharthakki/Pandesh_Releases/issues)
