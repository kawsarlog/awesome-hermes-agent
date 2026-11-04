<a id="top"></a>
# Profiles (many agents on one machine)

A **profile** is a separate Hermes home directory under `~/.hermes/profiles/`. Each profile has its own `config.yaml`, `.env`, `SOUL.md`, memories, sessions, skills, cron jobs, and state. Source: [Profiles docs](https://hermes-agent.nousresearch.com/docs/user-guide/profiles) (scraped 2026-11-04 Asia/Dhaka).

## Why profiles matter

Never point two running agent processes at the same profile. Both write memory and can mix each other's state. Use separate profiles for separate jobs (coding bot vs personal bot). Shared memory should use an [external memory provider](https://hermes-agent.nousresearch.com/docs/user-guide/features/memory-providers) instead.

When you create a profile named `coder`, Hermes also exposes commands like `coder chat`, `coder setup`, `coder gateway start`.

## Terms (official)

| Term | Meaning |
|------|---------|
| Profile | Persistent home for config and data |
| Agent | The running Hermes assistant using that home |
| Bot Mode bot | A profile shown in Desktop Bot Mode with avatar and Bot Chat |
| Messaging bot | A Telegram/Discord/Slack account connected via the gateway |
| Subagent | Child assistant from `delegate_task` for one job |

## Personality file

`SOUL.md` in `HERMES_HOME` is the primary identity (system prompt slot #1). Hermes seeds a default if missing and never overwrites an existing user file. Source: [Personality docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/personality).

```bash
hermes profile create research
hermes profile create research --no-skills   # blank slate skills
```

---

| | |
|:---|---:|
| [Community](community.md) ← | [Cron](cron.md) → |


