<a id="top"></a>
# Memory

<p align="center">
  <img src="../assets/sections/sec-memory.png" alt="Memory" width="100%">
</p>

## Official behavior

Hermes keeps persistent memory across sessions. It can search past conversations (FTS5 with LLM summarization) and build a deepening user model (including [Honcho](https://github.com/plastic-labs/honcho) dialectic modeling). Skills act as procedural memory. Sources: [memory docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/memory), [README](https://github.com/NousResearch/hermes-agent).

Stopping a local agent ends the process but does **not** delete saved conversations, memories, or skills. Source: [official FAQ](https://hermes-agent.nousresearch.com/).

## Files beginners hear about

Community and migration docs often mention persona / memory files such as `SOUL.md`, `MEMORY.md`, and `USER.md` (especially when importing from OpenClaw). Keep them short and honest. Sources: [OpenClaw migration](https://hermes-agent.nousresearch.com/docs/guides/migrate-from-openclaw), [personality docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/personality), [context files](https://hermes-agent.nousresearch.com/docs/user-guide/features/context-files).

## Treat skills and memory like code

Version useful skills. Review changes. Do not paste secrets into memory files. See [Medium: Git for Agent Memory](https://medium.com/@techlatest.net/git-for-agent-memory-why-you-should-treat-hermes-skills-like-code-61b03ed6f6b1).


## Official docs deep notes (2026-11-04)

Scraped from [memory feature docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/memory):

- Hermes stores lasting notes so later sessions can reuse project facts and preferences
- Keep memory files concise; stale or secret-looking lines should be deleted by you
- Skills complement memory as procedural "how I do this" knowledge (see [skills.md](skills.md))
- For managed user modeling, Honcho is the referenced dialectic layer ([plastic-labs/honcho](https://github.com/plastic-labs/honcho))

Always prefer the live docs page if this summary and upstream disagree.

## Optional memory backends (community)

| Project | Stars (2026-11-04 Asia/Dhaka) | Notes |
|---------|-------------------------------|-------|
| [vectorize-io/hindsight](https://github.com/vectorize-io/hindsight) | 58656 | Listed as Hermes memory plugin in community indexes |
| [plastic-labs/honcho](https://github.com/plastic-labs/honcho) | 7936 | Officially referenced user modeling library |
| [elkimek/honcho-self-hosted](https://github.com/elkimek/honcho-self-hosted) | 383 | Self-host Honcho for Hermes |

---

| | |
|:---|---:|
| [Skills](skills.md) ← | [Tools and MCP](tools-mcp.md) → |

