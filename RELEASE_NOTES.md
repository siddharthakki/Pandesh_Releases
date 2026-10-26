# Pandesh v0.1.4 Public Alpha — Build 145

**Release channel:** Alpha  
**Platform:** Windows 10/11 x64  
**Release source revision:** 2eeb5fae8a251e4dc00b45df9ebbef921b8dead3 ([siddharthakki/Pandesh@2eeb5fa](https://github.com/siddharthakki/Pandesh/commit/2eeb5fae8a251e4dc00b45df9ebbef921b8dead3))

## Highlights

- **Launcher Profile Alignment:** Aligned launcher default data directory with installed desktop (%LOCALAPPDATA%\\KarkeDikha\\desktop), ensuring credentials, model selection, and configurations are reliably preserved across launch methods.
- **Task Outcome Evidence Bounding & Deduplication:** Guarded background task outcome finalization by deduplicating tool calls and bounding evidence items to prevent metadata bloat, while preserving full underlying execution receipts.
- **Packaged Smoke & Upgrade Verification:** 14/14 packaged installer smoke tests passed cleanly in isolated runtime with verified in-place upgrade handling.

## Verification

- **14/14 packaged installer smoke tests passed** cleanly with headless CDP driver and isolated runtime environment.
- **Clean source state** at commit 2eeb5fae8a251e4dc00b45df9ebbef921b8dead3.

## Checksums (SHA-256)
27FD5698148273B0FE548060AA831F5F1944B531EF9F04F4F65AD2B043FEB639  Pandesh-Setup.exe
957211727ECCA4F2FF54E2F6754D55E548C5A311A19FFBD78C7BA0A8CC276A49  Pandesh-v0.1.4-alpha-win32-x64-portable.zip

---

# Pandesh v0.1.3 Public Alpha — Build 144

**Release channel:** Alpha  
**Platform:** Windows 10/11 x64  
**Release source revision:** 979394209ef7491d904b88e17812fa4b0fa0d65b ([siddharthakki/Pandesh@9793942](https://github.com/siddharthakki/Pandesh/commit/979394209ef7491d904b88e17812fa4b0fa0d65b))

## Highlights

- **Nonblocking Background Task Delegation:** Async background task delegation with verified recovery and truthful cancellation.
- **Installer & Process Hardening:** Hardened process isolation during smoke tests and upgrades; uninstaller runs with /NOCLOSEAPPLICATIONS preventing Windows Restart Manager interference.
- **Clean Verified Build:** Clean working tree verification with embedded build identity (Build 144) and full checksum manifests.

## Verification

- **14/14 packaged installer smoke tests passed** cleanly with headless CDP driver and isolated runtime environment.
- **Clean source state** at commit 9793942.

## Checksums (SHA-256)
5C1621346EA9D7946BB85A9B0BDA931DA43EC9E7B7F2FCA411825AA255494AAF  Pandesh-Setup.exe
DA0AE6F31B6E41D6C558230AC08663556C19C1B281C8EF38369117AB0FCAE68F  Pandesh-v0.1.3-alpha-win32-x64-portable.zip

---

# Pandesh v0.1.1 Public Alpha — Build 142

**Release channel:** Alpha  
**Platform:** Windows 10/11 x64  
**Release source revision:** `8166f627a3522493eb129ff8d91a1f164770a112` (private development repository)

## Highlights

- Local-first conversations through locally running Ollama models
- Governed task execution with approval before consequential actions
- Persistent memory, commitments, and scheduled assistant workflows
- Read-only system diagnostics
- Hardened process-ownership rules: safeguards against unintended process termination and PID reuse

## Verification

The development release report records **27/27 Windows Sandbox checks passing**, including an unrelated disposable process surviving installation, app startup, and shutdown. An isolated local-model acceptance journey using `qwen3-coder:swift-27b` exercised approved memory operations, recall, commitment persistence, and a scheduled briefing.

These are reported release-gate results, not a claim that every machine configuration or capability has been tested.

## Install

1. Download `Pandesh-Setup.exe` from the **Assets** section of this public release.
2. Compare its SHA-256 to the value in [SHA256SUMS.txt](https://github.com/siddharthakki/Pandesh_Releases/blob/main/SHA256SUMS.txt).
3. Install [Ollama](https://ollama.com/download) and download an appropriate model (`ollama pull qwen2.5-coder:3b` is one example).
4. Run the installer and launch Pandesh.

Alternatively extract `Pandesh-v0.1.1-alpha-win32-x64-portable.zip` and run `Launch-Pandesh.cmd`.

**Known limits:** unsigned installer (SmartScreen warning possible), locally running Ollama required, device-dependent microphone support, integrations requiring explicit permissions. This is an alpha; please report bugs.

**Feedback:** [GitHub Issues](https://github.com/siddharthakki/Pandesh_Releases/issues). Do not share sensitive data in bug reports.
