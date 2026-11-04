<a id="top"></a>
# Install Hermes Agent

<p align="center">
  <img src="../assets/sections/sec-install.png" alt="Install" width="100%">
</p>

Official source of truth: [Installation](https://hermes-agent.nousresearch.com/docs/getting-started/installation).

## One-liners (verified)

| Platform | Command |
|----------|---------|
| Linux / macOS / WSL2 | `curl -fsSL https://hermes-agent.nousresearch.com/install.sh \| bash` |
| Windows PowerShell | `iex (irm https://hermes-agent.nousresearch.com/install.ps1)` |
| Headless VPS (skip browser deps) | `curl -fsSL https://hermes-agent.nousresearch.com/install.sh \| bash -s -- --skip-browser` |

Sources: [README](https://github.com/NousResearch/hermes-agent), [Medium setup guide citing the same installers](https://medium.com/@techlatest.net/git-for-agent-memory-why-you-should-treat-hermes-skills-like-code-61b03ed6f6b1).

## After install

```bash
source ~/.bashrc    # or ~/.zshrc
hermes              # interactive CLI
hermes model        # choose provider and model
hermes setup        # full setup wizard
hermes setup --portal   # Nous Portal OAuth + Tool Gateway
hermes doctor       # diagnose issues
hermes update       # update to latest
```

Config lives under `~/.hermes/` on Linux/macOS/WSL2. Native Windows install lives under `%LOCALAPPDATA%\hermes`. Source: [README](https://github.com/NousResearch/hermes-agent).


## Desktop packages (official details)

From [installation docs](https://hermes-agent.nousresearch.com/docs/getting-started/installation) (scraped 2026-11-04 Asia/Dhaka):

- Download Desktop packages from the [Hermes website](https://hermes-agent.nousresearch.com/)
- **Windows:** open the `.appinstaller` with Windows App Installer (signed MSIX). Store packages are separate.
- **macOS:** open the DMG and copy `Hermes.app` to Applications. The macOS installer is **Apple Silicon only**. Intel macOS is unsupported per [platform support](https://hermes-agent.nousresearch.com/docs/getting-started/platform-support).
- Bundled packages include the agent, Python, and supported dependencies. Provider setup may still need network.
- To use Desktop with a Hermes backend on another machine: install Desktop, then connect from **Settings → Gateways** ([Desktop docs](https://hermes-agent.nousresearch.com/docs/user-guide/desktop#connecting-to-a-remote-backend)).

Full OS matrix: [Platform Support](https://hermes-agent.nousresearch.com/docs/getting-started/platform-support).

## Desktop and Termux

- **Desktop:** download from [hermes-agent.nousresearch.com](https://hermes-agent.nousresearch.com/) (macOS 12+, Windows 10/11, Linux).
- **Android / Termux:** use the [Termux guide](https://hermes-agent.nousresearch.com/docs/getting-started/termux), not the desktop/server installer script. A signed APT repository provides `stable` and `canary` channels. Source: [README](https://github.com/NousResearch/hermes-agent).

## Windows Defender note

Antivirus may flag bundled `uv.exe` (Astral's Python package manager) as a false positive. The official README explains how to verify the hash with GitHub attestation and how to whitelist the Hermes `bin` folder. Source: [README troubleshooting](https://github.com/NousResearch/hermes-agent).

## Community install helpers (optional)

These are community projects. Read each README and prefer isolated backends for untrusted work.

| Project | Notes | Stars (GitHub API, 2026-11-04 Asia/Dhaka) |
|---------|-------|---------------------------------------------|
| [xmbshwll/hermes-agent-docker](https://github.com/xmbshwll/hermes-agent-docker) | Minimal Docker sandbox image | 48 |
| [0xrsydn/nix-hermes-agent](https://github.com/0xrsydn/nix-hermes-agent) | Nix package and NixOS module | 48 |
| [42-evey/evey-setup](https://github.com/42-evey/evey-setup) | Opinionated stack setup | 73 |

## Migrating from OpenClaw or other agents

During `hermes setup`, Hermes can import from OpenClaw, Claude Code, Codex, or Cursor when it finds their folders. After install:

```bash
hermes plugins install agent-importers
hermes import-agent openclaw --dry-run
hermes import-agent openclaw
hermes import-agent claude-code   # or codex / cursor
```

Older spelling `hermes claw migrate` still works. Sources: [README](https://github.com/NousResearch/hermes-agent), [migrate from OpenClaw](https://hermes-agent.nousresearch.com/docs/guides/migrate-from-openclaw), [import from other agents](https://hermes-agent.nousresearch.com/docs/user-guide/import-from-other-agents).

---

| | |
|:---|---:|
| [Getting started](getting-started.md) ← | [Features](features.md) → |

