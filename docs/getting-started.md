<a id="top"></a>
# Getting started with Hermes Agent

<p align="center">
  <img src="../assets/sections/sec-getting-started.png" alt="Getting started" width="100%">
</p>

> [!NOTE]
> Short path from zero to a first chat. Full install details: [install.md](install.md). Official docs: [hermes-agent.nousresearch.com/docs](https://hermes-agent.nousresearch.com/docs/).

## What is Hermes Agent?

Hermes Agent is the self-improving AI agent built by [Nous Research](https://nousresearch.com). It has a built-in learning loop. It can create skills from experience, improve them while using them, search past conversations, and build a model of who you are across sessions. Source: [official README](https://github.com/NousResearch/hermes-agent) and [product site](https://hermes-agent.nousresearch.com/).

It is free and open source under the MIT license. Model providers and optional hosted services have their own pricing. Source: [official FAQ](https://hermes-agent.nousresearch.com/).

## What you need

- A computer: macOS, Linux, Windows (native or WSL2), or Android via Termux. Sources: [install docs](https://hermes-agent.nousresearch.com/docs/getting-started/installation), [Termux guide](https://hermes-agent.nousresearch.com/docs/getting-started/termux).
- A model provider (Nous Portal, OpenRouter, OpenAI, local endpoint, and others). Source: [providers](https://hermes-agent.nousresearch.com/docs/integrations/providers).
- Optional: Telegram, Discord, Slack, WhatsApp, Signal, or Email if you want the messaging gateway. Source: [README](https://github.com/NousResearch/hermes-agent).

## Checklist: install in a few minutes

### Linux, macOS, WSL2

```bash
curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash
source ~/.bashrc    # or: source ~/.zshrc
hermes              # start chatting
```

### Windows (PowerShell, native)

```powershell
iex (irm https://hermes-agent.nousresearch.com/install.ps1)
```

Native Windows runs CLI, gateway, TUI, and tools without WSL. Source: [README](https://github.com/NousResearch/hermes-agent).

### Desktop app

Hermes Desktop is available for macOS, Windows, and Linux from the [official site](https://hermes-agent.nousresearch.com/).

## Checklist: first useful chat

- [ ] Run `hermes` (or open Desktop)
- [ ] Run `hermes model` or `hermes setup --portal` to pick a provider
- [ ] Ask a safe question that changes nothing outside chat
- [ ] Run `hermes doctor` if something looks wrong
- [ ] Later: `hermes tools`, `hermes gateway`, and [skills](skills.md)

<details>
<summary><strong>Click: example first message</strong></summary>

<br>

```
You are my research helper.
Summarize what tools you currently have enabled.
Do not change any files or send any messages outside this chat.
```

</details>

## Skip collecting many API keys

If you want one login for models plus hosted tools (web search, images, speech, cloud browser), use Nous Portal:

```bash
hermes setup --portal
```

Then check with `hermes portal info`. Source: [README](https://github.com/NousResearch/hermes-agent), [Tool Gateway docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/tool-gateway).

## After the first win

1. Browse [skills.md](skills.md) and [agentskills.io](https://agentskills.io).
2. Read [memory.md](memory.md) so Hermes remembers your projects.
3. Try a workflow from [workflows.md](workflows.md).
4. Skim [security.md](security.md) before enabling risky tools or public chat gateways.

## Official links

| Topic | Link |
|------|------|
| Product site | [hermes-agent.nousresearch.com](https://hermes-agent.nousresearch.com/) |
| Docs home | [Docs](https://hermes-agent.nousresearch.com/docs/) |
| GitHub | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) |
| Nous Portal | [portal.nousresearch.com](https://portal.nousresearch.com) |
| Discord | [discord.gg/NousResearch](https://discord.gg/NousResearch) |

---

| | |
|:---|---:|
| [README](../README.md) ← | [Install](install.md) → |

