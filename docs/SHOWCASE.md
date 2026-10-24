# Pandesh v0.1.2 Build 143 — screenshots and interface fixes

**These screenshots show the updated v0.1.2 Alpha, Build 143 desktop app**, including fixes for New Conversation and Tasks & Results. The [currently public installer](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha) is still v0.1.1 Build 142 and does not necessarily include those fixes.

These are screenshots of **the actual updated Pandesh interface**, not old designs or mockups. The captured on-screen responses demonstrate presentation, but screenshots alone cannot certify each tool's underlying execution. A model name mentioned by the chat answer differs from the active model shown in the interface—an issue to validate separately, not a reason to dismiss the new UI screenshots.

[Download the public alpha](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha) · [Getting started](GETTING_STARTED.md) · [Architecture diagram](https://github.com/siddharthakki/Pandesh/blob/main/docs/ARCHITECTURE.md) · [Roadmap](https://github.com/siddharthakki/Pandesh/blob/main/docs/ROADMAP.md)

## Gallery

### 1. New conversation — Panda desktop

An empty-conversation UI with a pinned composer and local-model selector.

![Pandesh v0.1.2 Build 143 Panda desktop welcome screen](../assets/screenshots/01-welcome-chat.png)

### 2. AI models and provider connections

Settings surface for local/OpenAI-compatible and optional cloud providers. The displayed LAN endpoint is demo configuration.

![Pandesh desktop AI model provider settings in development Build 143](../assets/screenshots/02-local-model-connected.png)

### 3. Conversation preview

A conversation about local model availability; the returned model name differs from the selected model label. This model-self-awareness behavior needs separate validation.

![Pandesh desktop conversation demonstrating markdown and structured replies](../assets/screenshots/03-real-chat.png)

### 4. Diagnostics presentation

The updated UI renders a diagnostic result; the machine values shown have not been independently validated against the executing environment.

![Pandesh desktop diagnostic-results example with sample hardware values](../assets/screenshots/04-read-only-diagnostics.png)

### 5. Approval request presentation

Example request for a proposed `package.json` edit with a visible diff and Approve/Reject controls. An approval screen does not by itself establish execution.

![Pandesh desktop approval dialog showing a proposed package file edit](../assets/screenshots/05-real-approval-request.png)

### 6. Tasks and results

Build 143's one-click Results tab and artifact cards, addressing the earlier excessively long scrolling layout.

![Pandesh v0.1.2 Build 143 Tasks and Results navigation preview](../assets/screenshots/06-completed-tasks-and-results.png)

## Video walkthrough

**Not yet uploaded.** The public v0.1.1 release currently has no walkthrough MP4 asset. An earlier storyboard is a production plan, not a completed video.

A verified video should capture a clean demo session, keep private applications and notifications out of frame, demonstrate an actual Ollama model response and real tool evidence, and clearly distinguish sample data from live system measurements. See the [source project](https://github.com/siddharthakki/Pandesh) for development and contribution information.
