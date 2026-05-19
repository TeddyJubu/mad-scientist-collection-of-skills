# Mad Scientist Collection of Skills

<p align="center">
  <strong>A curated operating library of agent skills for real estate, research, media, infrastructure, automation, and software work.</strong>
</p>

<p align="center">
  <img alt="Skills" src="https://img.shields.io/badge/skills-205-111827?style=for-the-badge">
  <img alt="Categories" src="https://img.shields.io/badge/categories-12-7c3aed?style=for-the-badge">
  <img alt="Format" src="https://img.shields.io/badge/format-SKILL.md-2563eb?style=for-the-badge">
  <img alt="Quality" src="https://img.shields.io/badge/quality-validated-059669?style=for-the-badge">
</p>

---

## What This Is

Mad Scientist Collection of Skills is an organized library of reusable agent capabilities. Each skill is a self-contained folder with a `SKILL.md` entrypoint and optional scripts, references, examples, templates, or assets.

The collection is designed for agent runtimes such as Hermes Gateway, OpenClaw, Claude-style skill loaders, and any workflow that can discover and execute `SKILL.md` instructions.

## Collection Map

```text
Mad Scientist Collection of Skills
├── 01-real-estate             property research, skip tracing, rehab estimates
├── 02-content-social          YouTube, thumbnails, social posting, repurposing
├── 03-productivity            Notion, email, files, documents, PDFs
├── 04-devops-infrastructure   Docker, Traefik, Vercel, systemd, ports
├── 05-data-research           Apify, Census, Apollo, Brave, SEO, research
├── 06-ai-agents               agent workflows, voice, browser, OpenClaw
├── 07-image-graphics          image generation, editing, video, design
├── 08-communication           Discord and communication surfaces
├── 09-media-lifestyle         weather, TTS, audio, video, Spotify
├── 10-openclaw-mcp            OpenClaw platform and MCP client skills
├── 11-software-development    review, debugging, TDD, planning, agents
└── 12-tools                   broad utility bench: MLOps, creative, GitHub, email
```

## Category Index

| Area | Skills | Best for |
|---|---:|---|
| [`01-real-estate`](./01-real-estate) | 7 | Property lookup, skip tracing, repair estimates, investment reports |
| [`02-content-social`](./02-content-social) | 15 | YouTube growth, social posting, scripts, thumbnails, content reuse |
| [`03-productivity`](./03-productivity) | 9 | Notion, email, file delivery, document and PDF workflows |
| [`04-devops-infrastructure`](./04-devops-infrastructure) | 6 | Deployments, reverse proxying, Vercel, service health, port control |
| [`05-data-research`](./05-data-research) | 17 | Web research, data APIs, Census, Apify, Apollo, SEO, papers |
| [`06-ai-agents`](./06-ai-agents) | 21 | Agent operations, OpenClaw, outbound voice, browser automation |
| [`07-image-graphics`](./07-image-graphics) | 8 | Image generation, image editing, avatar video, Remotion, design |
| [`08-communication`](./08-communication) | 1 | Discord control |
| [`09-media-lifestyle`](./09-media-lifestyle) | 10 | TTS, video frames, transcripts, weather, music, media utilities |
| [`10-openclaw-mcp`](./10-openclaw-mcp) | 3 | OpenClaw platform operations and MCP tooling |
| [`11-software-development`](./11-software-development) | 12 | Code review, debugging, TDD, planning, subagent development |
| [`12-tools`](./12-tools) | 96 | General-purpose utilities across creative, MLOps, GitHub, email, docs |

## Featured Capabilities

| Skill | Location | What it does |
|---|---|---|
| `mad-skip-trace` | [`01-real-estate/mad-skip-trace`](./01-real-estate/mad-skip-trace) | Skip trace property addresses through BatchData |
| `nova-youtube-agent` | [`02-content-social/nova-youtube-agent`](./02-content-social/nova-youtube-agent) | Run YouTube growth onboarding, ideation, scripts, and feedback loops |
| `notion-mastery` | [`03-productivity/notion-mastery`](./03-productivity/notion-mastery) | Build structured Notion systems, pages, databases, and templates |
| `traefik-docker-deploy` | [`04-devops-infrastructure/traefik-docker-deploy`](./04-devops-infrastructure/traefik-docker-deploy) | Deploy Docker apps behind Traefik with SSL and routing guidance |
| `firehose` | [`05-data-research/firehose`](./05-data-research/firehose) | Monitor web mentions and real-time page streams |
| `openclaw-logo-maker` | [`06-ai-agents/openclaw-logo-maker`](./06-ai-agents/openclaw-logo-maker) | Generate polished logo variations with image models |
| `nano-banana-image-gen` | [`07-image-graphics/nano-banana-image-gen`](./07-image-graphics/nano-banana-image-gen) | Generate image assets with Gemini image models |
| `software-development` | [`11-software-development/software-development`](./11-software-development/software-development) | Review, debug, plan, and ship software with agent workflows |

## Skill Anatomy

Each skill should be easy for an agent to load and safe for a maintainer to inspect:

```text
skill-name/
├── SKILL.md       main instructions and metadata
├── scripts/       optional executable helpers
├── references/    API notes, examples, operational guides
├── templates/     reusable prompts, documents, or code shapes
├── assets/        static supporting assets
└── .env           local secrets only, never committed
```

Every `SKILL.md` starts with YAML frontmatter:

```yaml
---
name: example-skill
description: One clear sentence describing when and why to use this skill.
---
```

## Setup

Clone the collection:

```bash
git clone https://github.com/TeddyJubu/mad-scientist-collection-of-skills.git
cd mad-scientist-collection-of-skills
```

Store secrets outside git:

```bash
~/.hermes/skills/<skill>/.env
~/.hermes/.env
```

Use placeholders in committed docs and scripts:

```bash
API_KEY=your_api_key_here
```

## Quality Gates

The current collection has been checked for:

| Check | Status |
|---|---|
| `SKILL.md` frontmatter present | Passed |
| Unique skill names | Passed |
| JSON validity | Passed |
| Python syntax compilation | Passed |
| JavaScript syntax check | Passed |
| Shell syntax check | Passed |
| Bundled pytest suite | `109 passed, 8 skipped` |
| Obvious committed secret patterns | Clean, except masked examples |

## Maintenance Rules

- Keep `SKILL.md` focused on when to use the skill and how to operate it.
- Keep API keys, tokens, host passwords, and private environment values out of git.
- Prefer environment variables and `.env` examples with placeholder values.
- Add scripts only when they are reusable and parse cleanly.
- Avoid duplicate skill names; the `name` field should be stable and machine-friendly.
- Keep host-specific details parameterized with environment variables when possible.

## License

Private collection for Mad Scientist systems and related agent workflows.
