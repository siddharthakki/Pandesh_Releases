# Pandesh — Troubleshooting and FAQ

For **v0.1.1 Public Alpha (Build 142)**. [Start here](GETTING_STARTED.md) · [Downloads](../README.md)

## Pandesh says “No models found”

1. Open PowerShell and check that Ollama is installed: `ollama --version`.
2. Check installed models: `ollama list`.
3. If nothing is installed, try `ollama pull qwen2.5-coder:3b`.
4. Check the local service: `Invoke-RestMethod http://127.0.0.1:11434/api/tags`.
5. Restart Pandesh after confirming Ollama is reachable. Check provider/model settings if available.

Do **not** paste private access tokens or full configuration files into a public issue.

## I can chat, but Pandesh says it can't use local tools

This is a known type of alpha integration problem under investigation. A successful chat proves model inference, **not** capability discovery or tool execution. Check that the tool appears enabled in your configuration, then retry with a specific read-only request. If the assistant still gives manual terminal instructions instead of invoking an available tool, report the prompt and model.

## The model is too slow

Try a smaller model such as `qwen2.5-coder:3b`, close unnecessary GPU-heavy applications, and check Ollama's reported running models using `ollama ps`. Performance depends on CPU, GPU/VRAM, RAM, prompt size and model configuration. A larger model is not always the best interactive choice.

## The app won't launch, or closes unexpectedly

- Check your Windows version (Windows 10/11 x64).
- Confirm you extracted the **entire** portable ZIP before launching.
- Restart Windows if a previous installer session is still active.
- Avoid repeated installation attempts if other applications close unexpectedly.
- If unrelated apps are terminated, stop using Pandesh and report it with the app version, install versus ordinary startup, and approximate time. **Do not repeat the problem deliberately on your everyday PC.**

## A request shows “waiting for approval”

Read the exact action and scope before approving it. An approval means permission to attempt an action, not evidence that it finished. Verify completion in the task/result view.

## Gmail or Calendar fails

Those sources need explicit connection and authorization. A read-denied result means Pandesh did not access the source. Do not describe the denied action as complete. Check connected-service permissions and retry only after granting the appropriate scope.

## Do I need internet access?

Downloading Ollama models and setting up connected services typically requires internet. Once installed, local-model inference through Ollama can run locally, but web lookups and cloud-connected workflows need their respective connections.

## Is the installer signed?

No. This alpha is currently unsigned. Use only the [official GitHub release](https://github.com/siddharthakki/Pandesh_Releases/releases/tag/v0.1.1-pandesh-alpha), and verify its SHA-256 digest using [SHA256SUMS.txt](../SHA256SUMS.txt). An unfamiliar publisher warning does **not** prove a file is safe.

## How do I report a useful bug?

Open a [GitHub Issue](https://github.com/siddharthakki/Pandesh_Releases/issues) with:
- Version and build shown in Pandesh
- Windows version and hardware (CPU/GPU/RAM)
- Local model name and Ollama availability
- Exact steps to reproduce
- Expected behavior versus actual behavior
- A cropped, redacted screenshot or short screen recording, if useful

**Remove** email addresses, calendar details, file paths containing personal identifiers, tokens, browser tabs, taskbar notifications, and any other private content. Do not upload raw logs or your SQLite database.
