<a id="top"></a>
# Prompt library

<p align="center">
  <img src="../assets/sections/sec-prompts.png" alt="Prompt library" width="100%">
</p>

Safe starter prompts. They ask Hermes to explain or draft. They avoid sends, deletes, and purchases unless you change them on purpose.

## First session

```
List the tools you currently have enabled.
Explain each in one plain sentence.
Do not change files or call external APIs yet.
```

## Turn a finished job into a skill

```
We just finished a workflow together.
Create a reusable skill that captures the steps, inputs, and checks.
Show me the SKILL.md draft before saving anything.
```

## Daily briefing (then schedule)

```
Draft a morning briefing template for my projects.
Include: calendar risks, open PRs I mentioned before, and one learning note.
After I approve the template, help me schedule it with cron to Telegram.
```

## Security-minded review

```
Review this skill folder I am about to enable.
List tools it needs, files it touches, and any risky commands.
Do not run it yet.
```

## Subagent plan

```
Break this goal into independent workstreams.
Propose which parts a subagent should own.
Wait for my OK before spawning anyone.
```

## Memory hygiene

```
Summarize what you know about my preferences in MEMORY.md style.
Flag anything that looks secret or outdated so I can delete it.
```

More prompting tips: keep goals measurable, name the delivery channel, and say what "done" looks like (Hermes release notes describe evidence-based verification and `/goal` loops on community mirrors such as [hermesagents.net](https://hermesagents.net/); confirm on your installed version).

---

| | |
|:---|---:|
| [Shortcuts](shortcuts.md) ← | [Glossary](glossary.md) → |

