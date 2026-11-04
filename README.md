# Awesome Hermes Agent

<p align="center">
  <img src="assets/cover.jpg" alt="Awesome Hermes Agent" width="100%">
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge-flat.svg" alt="Awesome"></a>
  <a href="https://github.com/NousResearch/hermes-agent"><img src="https://img.shields.io/github/stars/NousResearch/hermes-agent?style=flat-square&label=hermes-agent&color=F0A020" alt="Hermes Agent stars"></a>
  <img src="https://img.shields.io/badge/Beginner-guide-FFE14A?style=flat-square&labelColor=121212" alt="Beginner guide">
  <img src="https://img.shields.io/badge/License-CC0-lightgrey?style=flat-square" alt="License">
</p>

<p align="center">
  <strong>Beginner guides + curated links for <a href="https://github.com/NousResearch/hermes-agent">Hermes Agent</a></strong><br>
  Independent community list. Not an official Nous Research project.
</p>

---

## TL;DR

Hermes Agent (by [Nous Research](https://nousresearch.com)) is a self-improving open-source agent. It keeps memory, learns skills, chats on Telegram/Discord/Slack/WhatsApp/Signal/Email/CLI, runs cron jobs, supports MCP, and can live on a VPS or serverless sandbox.

- Site: [hermes-agent.nousresearch.com](https://hermes-agent.nousresearch.com/)
- Docs: [hermes-agent.nousresearch.com/docs](https://hermes-agent.nousresearch.com/docs/)
- Code: [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)

---

## Contents

- [Quick start](#quick-start)
- [Who is it for](#who-is-it-for)
- [Why it is useful](#why-it-is-useful)
- [Guides](#guides)
- [Official links](#official-links)
- [Popular ecosystem](#popular-ecosystem)
- [Community indexes](#community-indexes)
- [FAQ](#faq)
- [License](#license)

---

## Quick start

```bash
# macOS / Linux / WSL2
curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash
source ~/.bashrc   # or ~/.zshrc
hermes
hermes setup --portal   # or: hermes model
hermes doctor
```

```powershell
# Windows PowerShell (native)
iex (irm https://hermes-agent.nousresearch.com/install.ps1)
```

Or install [Hermes Desktop](https://hermes-agent.nousresearch.com/).

More detail: [docs/getting-started.md](docs/getting-started.md) · [docs/install.md](docs/install.md)

---

## Who is it for

| You want... | Start here |
|-------------|------------|
| First install | [Getting started](docs/getting-started.md) |
| Ordered learning | [Learning path](docs/learning-path.md) |
| Skills safely | [Skills](docs/skills.md) |
| Hosting / VPS | [Deployments](docs/deployments.md) |
| Migrate from OpenClaw etc. | [Comparisons](docs/comparisons.md) |
| Stay safe | [Security](docs/security.md) |

---

## Why it is useful

1. Skills learning loop ([docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills))
2. Persistent memory ([docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/memory))
3. Many chat surfaces ([site](https://hermes-agent.nousresearch.com/))
4. Cron + MCP + Tool Gateway
5. Import from OpenClaw / Claude Code / Codex / Cursor ([migrate](https://hermes-agent.nousresearch.com/docs/guides/migrate-from-openclaw))
6. MIT license, bring your own models

<p align="center">
  <img src="assets/diagrams/diag-learning-loop.png" alt="Learning loop" width="100%">
</p>

<p align="center">
  <img src="assets/diagrams/diag-messaging.png" alt="Many surfaces" width="100%">
</p>

---

## Guides

| Guide | Topic |
|-------|-------|
| [getting-started](docs/getting-started.md) | First win |
| [install](docs/install.md) | Platforms, Desktop, Termux, migration |
| [features](docs/features.md) | Feature map |
| [skills](docs/skills.md) | Skills + 1000+ star table |
| [memory](docs/memory.md) | Memory and Honcho |
| [tools-mcp](docs/tools-mcp.md) | Tools, MCP, Tool Gateway |
| [workflows](docs/workflows.md) | Example flows |
| [profiles](docs/profiles.md) | Multiple agents |
| [cron](docs/cron.md) | Scheduled jobs |
| [shortcuts](docs/shortcuts.md) | Commands |
| [prompt-library](docs/prompt-library.md) | Copy-paste prompts |
| [security](docs/security.md) | Approvals and trust |
| [troubleshooting](docs/troubleshooting.md) | Fixes |
| [comparisons](docs/comparisons.md) | Migration notes |
| [deployments](docs/deployments.md) | Hosting |
| [resources](docs/resources.md) | Link hub |
| [community](docs/community.md) | Discord and lists |
| [faq](docs/faq.md) | Common questions |
| [glossary](docs/glossary.md) | Terms |
| [limits](docs/limits.md) | Honest limits |
| [cheat-sheet](docs/cheat-sheet.md) | One page |
| [learning-path](docs/learning-path.md) | Study order |

---

## Official links

| | |
|--|--|
| <img src="assets/thumbs/card-official-docs.png" width="140" alt=""> | [Docs](https://hermes-agent.nousresearch.com/docs/) |
| <img src="assets/thumbs/card-nous-portal.png" width="140" alt=""> | [Nous Portal](https://portal.nousresearch.com) |
| <img src="assets/thumbs/card-skills-hub.png" width="140" alt=""> | [agentskills.io](https://agentskills.io) |
| <img src="assets/thumbs/card-discord.png" width="140" alt=""> | [Discord](https://discord.gg/NousResearch) |

Also: [Product site](https://hermes-agent.nousresearch.com/) · [GitHub](https://github.com/NousResearch/hermes-agent)

---

## Popular ecosystem

Full tables with fetch date: [docs/skills.md](docs/skills.md)

Highlights (GitHub API, 2026-11-04 Asia/Dhaka):

| Stars | Project |
|------:|---------|
| 260k+ | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) |
| 19k+ | [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) |
| 14k+ | [fathah/hermes-desktop](https://github.com/fathah/hermes-desktop) |
| 6k+ | [outsourc-e/hermes-workspace](https://github.com/outsourc-e/hermes-workspace) |
| 6k+ | [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) |

> [!IMPORTANT]
> Listings are discovery aids, not security badges. Read [security.md](docs/security.md) before enabling community skills.

---

## Community indexes

- [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent)
- [frankxai/awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents)
- [0xarkstar/awesome-hermes-agent](https://github.com/0xarkstar/awesome-hermes-agent)
- [get-hermes.ai/community](https://get-hermes.ai/community/)
- [AgentSkillsHub Hermes filter](https://agentskillshub.top/?search=Hermes&tab=explore&min_stars=1000)
- [hermesagents.net](https://hermesagents.net/)

---

## FAQ

<details>
<summary><strong>Is this official?</strong></summary>

<br>

No. Independent community guide. Official docs: [hermes-agent.nousresearch.com/docs](https://hermes-agent.nousresearch.com/docs/).

</details>

<details>
<summary><strong>Is Hermes free?</strong></summary>

<br>

The agent is MIT and free to self-host. Model APIs and optional Nous Portal tiers have their own pricing. Source: [official site](https://hermes-agent.nousresearch.com/).

</details>

More: [docs/faq.md](docs/faq.md)

---

## License

[CC0-1.0](LICENSE) for this list's original text. Linked projects keep their own licenses. Hermes Agent is MIT (upstream).
