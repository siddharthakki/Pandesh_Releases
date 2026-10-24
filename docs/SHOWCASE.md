# Pandesh screenshots and demo

[← Pandesh home](../README.md) · [Getting started](GETTING_STARTED.md)

## Real application screenshots

**Capture pending.** The existing design mockups are **not** screenshots of the released Windows application. This page will show genuine captures from **Pandesh v0.1.1 / Build 142** after a privacy review.

Planned gallery, captured from the installed alpha:

1. **Welcome / chat** — Panda interface, clear empty conversation, pinned composer
2. **Local model connected** — truthful selected model and provider status
3. **Read-only diagnostics** — actual tool call and evidence-backed result
4. **Approval workflow** — real pending approval with visible scope and decision controls
5. **Completed task** — result after approval, with real completion evidence
6. **Settings / About** — version, build number, runtime identity, provider configuration

## Walkthrough video

**Actual screen recording pending.** The short walkthrough will show a clean Windows desktop/app window, the launch and Ollama connection, a real chat, an actual tool result, and an approval lifecycle. No simulated successes or fabricated Gmail/calendar activity.

While the video is being prepared, follow the written [getting-started guide](GETTING_STARTED.md).

## Capture/privacy requirements for maintainers

- Record a **clean demo Windows account or isolated VM** using synthetic/demo data. Never show real mail, messages, documents, tokens, or calendar events.
- Capture the **Pandesh app window only**. Keep taskbar, notifications, browser tabs, other applications, and system tray out of the recording.
- Use an actual v0.1.1 alpha installer. Verify the displayed build before capture.
- Set window size consistently (e.g., 1440×900 or 1600×900); keep text readable.
- Do not portray a mockup, animation, or prerecorded tool result as live product behavior.
- For screenshots, prefer PNG/WebP. Optimize for GitHub page load; add descriptive alternate text.
- For video, record at 1080p, then publish the MP4 to a public video host or attach it to a GitHub release where size limits permit. Provide captions and a concise title/description.
- Show at least one failure or approval-rejection safeguard accurately when relevant.
- Review every frame and audio segment for personal information before publishing.

### Suggested 75–90-second demo storyboard

| Time | Scene | Demonstrate |
| --- | --- | --- |
| 0–10s | Title and opening Pandesh window | Genuine installed alpha, build 142 |
| 10–25s | Ollama status + conversation | Local model responds |
| 25–45s | Read-only diagnostics request | Real tool call, real returned results |
| 45–65s | Approval request | Meaningful approval summary, reject/approve path |
| 65–80s | Verified completion and task state | Observable outcome, not a fabricated success |
| 80–90s | Download / feedback | Public release URL |

Once captures are available, store screenshots under `assets/screenshots/` and replace this page's pending entries with real embedded images. Keep video upload links here and in the repository README.
