<a id="top"></a>
# Shortcuts and common commands

Official CLI reference: [CLI commands](https://hermes-agent.nousresearch.com/docs/reference/cli-commands).

## Everyday CLI

| Command | Purpose |
|---------|---------|
| `hermes` | Interactive chat / TUI |
| `hermes model` | Pick provider and model |
| `hermes tools` | Enable/disable tools |
| `hermes setup` | Full setup wizard |
| `hermes setup --portal` | Nous Portal login + Tool Gateway |
| `hermes portal info` | Show Portal wiring |
| `hermes gateway` / `hermes gateway setup` / `hermes gateway start` | Messaging bridge |
| `hermes mcp` | Curated MCP catalog picker |
| `hermes doctor` | Diagnose problems |
| `hermes update` | Update Hermes |
| `hermes config get` / `hermes config set` | Config values |
| `hermes plugins install ...` | Install plugins |
| `hermes import-agent ...` | Import from other agents |

## Shared slash commands (CLI and many messaging surfaces)

| Slash | Purpose |
|-------|---------|
| `/new` or `/reset` | Fresh conversation |
| `/model` | Change model |
| `/personality` | Set personality |
| `/retry` / `/undo` | Retry or undo last turn |
| `/compress` | Compress context |
| `/usage` / `/insights` | Usage insights |
| `/skills` | Browse skills |
| `/handoff` | Hand off mid-session (when available in your version) |
| `/stop` | Interrupt on messaging platforms |

Sources: [README](https://github.com/NousResearch/hermes-agent), [hermesagents.net command table](https://hermesagents.net/). Features vary by version. Run `hermes update` and check [releases](https://github.com/NousResearch/hermes-agent/releases).

---

| | |
|:---|---:|
| [Comparisons](comparisons.md) ← | [Prompt library](prompt-library.md) → |

