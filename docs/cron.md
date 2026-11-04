<a id="top"></a>
# Cron and scheduled jobs

Official source: [Cron docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/cron) (scraped 2026-11-04 Asia/Dhaka).

## What cron can do

- One-shot or recurring tasks
- Pause, resume, edit, trigger, remove
- Stop an in-flight run without deleting the schedule
- Attach zero or more skills to a job
- Deliver to origin chat, files, or platforms
- **No-agent mode:** run a script on a schedule with stdout delivered and no LLM call
- **Event triggers:** webhooks can fire a job when something happens (see messaging webhooks docs)

You can manage jobs in plain language (Hermes uses `cronjob_manage`) or with slash commands such as:

```bash
/cron add "in 30m" "Remind me to check the build"
```

## Which model a job uses

Resolution at fire time:

1. Per-job model pin (if set)
2. Else `cron.model` in config
3. Else the main agent model from `hermes model`

`hermes setup --portal` is the lowest-friction option for unattended runs because OAuth refresh is automatic.

## Safety notes

- Cron-run sessions cannot create more cron jobs (prevents runaway loops)
- Prefer approvals and allowlists when delivery hits public chat apps ([security](security.md))

---

| | |
|:---|---:|
| [Profiles](profiles.md) ← | [Cheat sheet](cheat-sheet.md) → |


