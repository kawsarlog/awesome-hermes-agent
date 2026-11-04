<a id="top"></a>
# Skills and the learning loop

<p align="center">
  <img src="../assets/sections/sec-skills.png" alt="Skills" width="100%">
</p>

## What a skill is

A skill is procedural memory: a reusable folder (usually with `SKILL.md`) that teaches Hermes how to do a job the same way next time. Hermes can create skills from experience and improve them during use. Skills are compatible with the open [agentskills.io](https://agentskills.io) standard. Sources: [skills docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills), [creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills), [README](https://github.com/NousResearch/hermes-agent).

Treat skills like code: review them, version them, and do not install random ZIPs without reading the source. That idea is also covered in [Git for Agent Memory (Medium)](https://medium.com/@techlatest.net/git-for-agent-memory-why-you-should-treat-hermes-skills-like-code-61b03ed6f6b1).

## How skills work (official)

Skills are on-demand knowledge documents Hermes loads when needed. They use **progressive disclosure** to save tokens and follow the [agentskills.io specification](https://agentskills.io/specification).

- Primary folder: `~/.hermes/skills/` (bundled, hub-installed, and agent-created skills live here)
- Optional external skill directories can be scanned too
- Every installed skill is available as a slash command (example pattern: `/skill-name ...`)
- Public Skills Hub cards can open Desktop via `hermes://skill/install?...` and run a security scan before install
- Blank slate: `hermes profile create NAME --no-skills` or `hermes skills opt-out` (and `opt-in --sync` to restore)

Catalogs: [Bundled skills](https://hermes-agent.nousresearch.com/docs/reference/skills-catalog), [Optional skills](https://hermes-agent.nousresearch.com/docs/reference/optional-skills-catalog), hub UI at [docs/skills](https://hermes-agent.nousresearch.com/docs/skills).

Source: [Skills feature docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills) (scraped 2026-11-04 Asia/Dhaka).

## Official starting points

| Resource | Why |
|----------|-----|
| [Skills docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills) | How skills work inside Hermes |
| [agentskills.io](https://agentskills.io) | Cross-agent skill standard and hub |
| [Official skills nav](https://hermes-agent.nousresearch.com/docs/skills) | Skills section in official docs site |
| [NousResearch/hermes-agent-self-evolution](https://github.com/NousResearch/hermes-agent-self-evolution) | DSPy + GEPA research for evolving skills/prompts |

## Trust boundary (read before installing)

An ecosystem listing is discovery help, not a security badge. Before enabling a community skill:

- Who can trigger it?
- Which tools can it use?
- Where do commands run (local vs Docker vs SSH)?
- What credentials can it read?
- How do you stop it?

Prefer the smallest toolset and an isolated backend for untrusted work. Official controls: [security](https://hermes-agent.nousresearch.com/docs/user-guide/security), [tools](https://hermes-agent.nousresearch.com/docs/user-guide/features/tools), [cron](https://hermes-agent.nousresearch.com/docs/user-guide/features/cron). Community scanners such as [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) can help review skill packages.

## From AgentSkillsHub (Hermes search, 1000+ stars filter)

Browse: [agentskillshub.top Hermes filter](https://agentskillshub.top/?search=Hermes&tab=explore&min_stars=1000) (scraped with JS wait 2026-11-04 Asia/Dhaka). Hub grades are their own SAFE/CAUTION labels, not Nous endorsements. Star counts below re-checked on GitHub API the same day.

| Stars (GitHub API) | Project | Hub note |
|-------------------:|---------|----------|
| 260414 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | Listed on Hub as Hermes Agent |
| 112423 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | Hub says works with Hermes among other agents |
| 110972 | [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | Manage agents at work; pairs with official paperclip adapter |
| 6823 | [anysearch-ai/anysearch-skill](https://github.com/anysearch-ai/anysearch-skill) | Hub tags include hermes / openclaw |
| 151741 | [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | Appears in Hub Hermes explore results |
| 105857 | [nexu-io/open-design](https://github.com/nexu-io/open-design) | Appears in Hub Hermes explore results |

Other Hub hits mentioning Hermes (verify before install): `colbymchenry/codegraph`, `anysearch-ai/anysearch-mcp-server`, `ZiChuanLan/agent-purge`, `stablyai/orca`, `MemoriLabs/Memori`, `rohitg00/agentmemory`. Open each GitHub page and re-check stars/maintenance.

## Discovery indexes

| Index | Focus |
|-------|-------|
| [AgentSkillsHub Hermes search (1000+ stars filter)](https://agentskillshub.top/?search=Hermes&tab=explore&min_stars=1000) | Large security-graded directory (JS UI). Use it to explore, then verify on GitHub. |
| [getclawcloud.com/skills](https://getclawcloud.com/skills) | Awesome Hermes Skills collection (Wavespeed, Skill Health Check, FFmpeg, and more) |
| [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) | Broad independent ecosystem directory |
| [frankxai/awesome-hermes-agent](https://github.com/frankxai/awesome-hermes-agent) | Web-first agents/UIs/tools index |
| [frankxai/awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills) | Skills companion list + safety gate notes |
| [0xarkstar/awesome-hermes-agent](https://github.com/0xarkstar/awesome-hermes-agent) | Another curated awesome list |
| [get-hermes.ai/community](https://get-hermes.ai/community/) | Community map of projects |

> [!NOTE]
> AgentSkillsHub pages are client-rendered. For this repo we still verify every listed GitHub repo with the public GitHub API and we print the fetch date next to star counts.

## Popular Hermes-related skills and repos (1000+ stars)

**Fetched:** 2026-11-04, Asia/Dhaka, via GitHub API. Threshold: 1000+ stars. Sorted high to low. Descriptions shortened from GitHub. Re-check stars before you depend on a project. Dropped entries that 404'd or no longer match their old awesome-list identity.

### Core and official

| Stars | Project | Why it matters |
|------:|---------|----------------|
| 260410 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | The agent itself |
| 26928 | [agentskills/agentskills](https://github.com/agentskills/agentskills) | Agent Skills specification |
| 187266 | [anthropics/skills](https://github.com/anthropics/skills) | Public Agent Skills examples (portable pattern Hermes also uses via agentskills.io) |
| 5637 | [NousResearch/hermes-agent-self-evolution](https://github.com/NousResearch/hermes-agent-self-evolution) | Evolutionary skill/prompt improvement |
| 2031 | [NousResearch/hermes-paperclip-adapter](https://github.com/NousResearch/hermes-paperclip-adapter) | Run Hermes as a managed Paperclip worker |
| 1662 | [NousResearch/autonovel](https://github.com/NousResearch/autonovel) | Long-form writing pipeline on Hermes |

### Skills packs and methodology (Hermes-compatible / listed in Hermes ecosystem guides)

| Stars | Project | Why it matters |
|------:|---------|----------------|
| 312132 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills framework and methodology (widely cited in Hermes awesome lists) |
| 139031 | [garrytan/gstack](https://github.com/garrytan/gstack) | Opinionated product/design/QA skill stack |
| 113161 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Production engineering skills for coding agents |
| 105857 | [nexu-io/open-design](https://github.com/nexu-io/open-design) | Design agent workspace with first-class Hermes support (per community indexes) |
| 35552 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | Large MITRE-mapped security skill set (agentskills.io style) |
| 27871 | [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | Persistent markdown planning skill pattern |
| 24287 | [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Scan skills before they run |
| 21848 | [jnMetaCode/agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) | Large role pack; community lists note Hermes among supported tools |
| 10566 | [Agents365-ai/drawio-skill](https://github.com/Agents365-ai/drawio-skill) | Natural language to draw.io; Hermes support noted upstream |
| 8463 | [jnMetaCode/superpowers-zh](https://github.com/jnMetaCode/superpowers-zh) | Chinese-enhanced superpowers pack listing Hermes among targets |
| 5414 | [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | Audit/rewrite AI writing patterns; Hermes-compatible per community |
| 31516 | [garrytan/gbrain](https://github.com/garrytan/gbrain) | Opinionated Hermes/OpenClaw brain config |
| 2743 | [AMAP-ML/SkillClaw](https://github.com/AMAP-ML/SkillClaw) | Evolve/dedupe skills from session data |
| 2579 | [wondelai/skills](https://github.com/wondelai/skills) | Broad agentskills.io library often recommended for Hermes |
| 1166 | [ZeroPointRepo/youtube-skills](https://github.com/ZeroPointRepo/youtube-skills) | YouTube transcript skills for agents |

### Memory providers (1000+)

| Stars | Project | Why it matters |
|------:|---------|----------------|
| 58656 | [vectorize-io/hindsight](https://github.com/vectorize-io/hindsight) | Agent memory system; community indexes list Hermes plugin path |
| 7936 | [plastic-labs/honcho](https://github.com/plastic-labs/honcho) | User modeling / memory library used with Hermes |

### UIs and operator surfaces (1000+)

| Stars | Project | Why it matters |
|------:|---------|----------------|
| 19388 | [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) | Popular web + phone UI for Hermes |
| 151741 | [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | Multi-CLI desktop assistant including Hermes (per description) |
| 34030 | [iOfficeAI/AionUi](https://github.com/iOfficeAI/AionUi) | 24/7 cowork app listing Hermes among engines |
| 14527 | [fathah/hermes-desktop](https://github.com/fathah/hermes-desktop) | Desktop companion |
| 11679 | [EKKOLearnAI/ekko-studio](https://github.com/EKKOLearnAI/ekko-studio) | Local-first multi-agent workspace (formerly listed as hermes-web-ui / studio in community indexes) |
| 6793 | [outsourc-e/hermes-workspace](https://github.com/outsourc-e/hermes-workspace) | Chat, terminal, memory, skills manager |
| 6442 | [builderz-labs/mission-control](https://github.com/builderz-labs/mission-control) | Self-hosted control plane / fleet dashboard |
| 2939 | [qingchencloud/clawpanel](https://github.com/qingchencloud/clawpanel) | Multi-engine panel for OpenClaw and Hermes |
| 2036 | [dodo-reach/hermes-desktop](https://github.com/dodo-reach/hermes-desktop) | Mac SSH-native Hermes workspace |
| 1851 | [joeynyc/hermes-hudui](https://github.com/joeynyc/hermes-hudui) | Consciousness / state monitor UI |
| 1805 | [Eynzof/Hermes-CN-Desktop](https://github.com/Eynzof/Hermes-CN-Desktop) | Chinese-community Tauri desktop app |
| 1775 | [abundantbeing/hermes-browser-extension](https://github.com/abundantbeing/hermes-browser-extension) | Browser side panel |
| 1645 | [uzairansaruzi/hermex](https://github.com/uzairansaruzi/hermex) | Native iPhone client |
| 3495 | [njbrake/agent-of-empires](https://github.com/njbrake/agent-of-empires) | Multi-agent orchestrator (Hermes among engines) |
| 1320 | [greyhaven-ai/autocontext](https://github.com/greyhaven-ai/autocontext) | Self-improving harness with Hermes CLI support |

### Guides and directories (1000+)

| Stars | Project | Why it matters |
|------:|---------|----------------|
| 5954 | [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) | Large independent ecosystem directory |
| 5049 | [alchaincyf/hermes-agent-orange-book](https://github.com/alchaincyf/hermes-agent-orange-book) | Beginner-to-expert Chinese practical guide |
| 1339 | [ksimback/hermes-ecosystem](https://github.com/ksimback/hermes-ecosystem) | Hermes Atlas community map |

### Under 1000 but useful Hermes-native starters

Listed because official/community getting-started paths mention them often (stars from same snapshot):

| Stars | Project |
|------:|---------|
| 560 | [Romanescu11/hermes-skill-factory](https://github.com/Romanescu11/hermes-skill-factory) |
| 544 | [42-evey/hermes-plugins](https://github.com/42-evey/hermes-plugins) |
| 514 | [Cranot/super-hermes](https://github.com/Cranot/super-hermes) |
| 380 | [witt3rd/oh-my-hermes](https://github.com/witt3rd/oh-my-hermes) |
| 276 | [tlehman/litprog-skill](https://github.com/tlehman/litprog-skill) |
| 136 | [black-forest-labs/skills](https://github.com/black-forest-labs/skills) |

## Link problems found while building this page

| URL / repo | Status | Action |
|------------|--------|--------|
| `therohitdas/youtube-skills` | GitHub 404 | Use [ZeroPointRepo/youtube-skills](https://github.com/ZeroPointRepo/youtube-skills) |
| `Rainhoole/hermes-agent-acp-skill` | GitHub 404 | Dropped |
| `ellickjohnson/portainer-stack-hermes` | GitHub 404 | Dropped |
| `SamurAIGPT/awesome-hermes-agent` | Resolves to unrelated email infra repo | Not listed as an awesome Hermes directory |

---

| | |
|:---|---:|
| [Features](features.md) ← | [Memory](memory.md) → |

