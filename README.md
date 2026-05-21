# Mad Scientist Collection of Skills

<p align="center">
  <strong>A curated operating library of client-ready agent skills for real estate, research, media, infrastructure, automation, and creative work.</strong>
</p>

<p align="center">
  <img alt="Skills" src="https://img.shields.io/badge/skills-55-111827?style=for-the-badge">
  <img alt="Categories" src="https://img.shields.io/badge/categories-9-7c3aed?style=for-the-badge">
  <img alt="Format" src="https://img.shields.io/badge/format-SKILL.md-2563eb?style=for-the-badge">
  <img alt="Quality" src="https://img.shields.io/badge/quality-validated-059669?style=for-the-badge">
</p>

---

## What This Is

Mad Scientist Collection of Skills is an organized library of reusable agent capabilities. Each skill is a self-contained folder with a `SKILL.md` entrypoint and optional scripts, references, examples, templates, or assets.

This cleaned edition removes system/default skills that should not be presented as client giveaway skills.

## AI Agent Install Guide

Use this repository when your agent can scan nested folders for `SKILL.md` files. Installing means making the skill folders available to the agent; do not execute every script during install.

### 1. Clone

```bash
git clone https://github.com/TeddyJubu/mad-scientist-collection-of-skills.git
cd mad-scientist-collection-of-skills
```

### 2. Validate Before Loading

```bash
test "$(find . -name SKILL.md | wc -l | tr -d ' ')" = "55"
```

### 3. Install For A Recursive Skill Loader

```bash
export AGENT_SKILLS_ROOT="${AGENT_SKILLS_ROOT:-$HOME/.hermes/skills}"
mkdir -p "$AGENT_SKILLS_ROOT/mad-scientist-collection"
rsync -a --delete --exclude ".git" --exclude ".env" --exclude "*.env" --exclude "__pycache__" --exclude "*.pyc" ./ "$AGENT_SKILLS_ROOT/mad-scientist-collection/"
```

## Collection Map

- `01-real-estate` (7 skills): Property research, owner lookup, skip tracing, repair estimates, and real estate workflows
- `02-content-social` (15 skills): YouTube, social posting, content repurposing, thumbnails, scripts, and marketing assets
- `03-productivity` (3 skills): Notion, email, Google Workspace, document, and PDF workflows
- `04-devops-infrastructure` (2 skills): Deployment, hosting, Docker, Vercel, and infrastructure workflows
- `05-data-research` (8 skills): Web research, public data, search, scraping, SEO, and source collection
- `06-ai-agents` (6 skills): Agent operations, voice workflows, browser automation, and agent setup
- `07-image-graphics` (5 skills): Image generation, editing, design, avatars, video, and visual production
- `09-media-lifestyle` (3 skills): Weather, audio, YouTube transcripts, and media utility workflows
- `12-tools` (6 skills): General-purpose utilities across ML, GitHub, email, creative production, and operations

## Category Index

| Area | Skills | Best for |
|---|---:|---|
| [`01-real-estate`](./01-real-estate) | 7 | Property research, owner lookup, skip tracing, repair estimates, and real estate workflows |
| [`02-content-social`](./02-content-social) | 15 | YouTube, social posting, content repurposing, thumbnails, scripts, and marketing assets |
| [`03-productivity`](./03-productivity) | 3 | Notion, email, Google Workspace, document, and PDF workflows |
| [`04-devops-infrastructure`](./04-devops-infrastructure) | 2 | Deployment, hosting, Docker, Vercel, and infrastructure workflows |
| [`05-data-research`](./05-data-research) | 8 | Web research, public data, search, scraping, SEO, and source collection |
| [`06-ai-agents`](./06-ai-agents) | 6 | Agent operations, voice workflows, browser automation, and agent setup |
| [`07-image-graphics`](./07-image-graphics) | 5 | Image generation, editing, design, avatars, video, and visual production |
| [`09-media-lifestyle`](./09-media-lifestyle) | 3 | Weather, audio, YouTube transcripts, and media utility workflows |
| [`12-tools`](./12-tools) | 6 | General-purpose utilities across ML, GitHub, email, creative production, and operations |

## Featured Capabilities

| Skill | Location | What it does |
|---|---|---|
| `batchdata-skip-trace` | [`01-real-estate/batchdata-skip-trace`](./01-real-estate/batchdata-skip-trace) | Skip trace property addresses to get owner information using the BatchData API. Use when Charles or Bob needs  |
| `homedepot-repair-estimator` | [`01-real-estate/homedepot-repair-estimator`](./01-real-estate/homedepot-repair-estimator) | Analyze property images, identify needed repairs, and generate contractor-style material estimates with Home D |
| `landglide-lookup` | [`01-real-estate/landglide-lookup`](./01-real-estate/landglide-lookup) | Look up US property parcel data via the ReportAll USA / LandGlide API. Query by address, parcel ID, owner name |
| `mad-skip-trace` | [`01-real-estate/mad-skip-trace`](./01-real-estate/mad-skip-trace) | Skip trace a property address through the BatchData API to find owner names, phone numbers, emails, alternate  |
| `owner-skip-trace` | [`01-real-estate/owner-skip-trace`](./01-real-estate/owner-skip-trace) | Skip trace a property owner by name and address using public web sources — free, no paid databases needed. Fin |
| `rentcast-property-report` | [`01-real-estate/rentcast-property-report`](./01-real-estate/rentcast-property-report) | Generates a comprehensive property analysis and investment report for a given US address using the Rentcast AP |
| `sdat-property-search` | [`01-real-estate/sdat-property-search`](./01-real-estate/sdat-property-search) | Search Maryland SDAT Real Property database for property owner, assessment, and tax info — no login required.  |
| `Content Repurposer` | [`02-content-social/Content Repurposer`](./02-content-social/Content Repurposer) | Turn one piece of content into 10+ formats. Transform blog posts, podcasts, videos, or talks into tweets, Link |
| `blotato-text-poster` | [`02-content-social/blotato-text-poster`](./02-content-social/blotato-text-poster) | Post text-only content (X threads, text posts) to social platforms via the Blotato v2 API. |
| `content-repurposing-engine` | [`02-content-social/content-repurposing-engine`](./02-content-social/content-repurposing-engine) | Turn one piece of content into 10+ formats. Transform blog posts, podcasts, videos, or talks into tweets, Link |
| `copywriting` | [`02-content-social/copywriting`](./02-content-social/copywriting) | When the user wants to write, rewrite, or improve marketing copy for any page — including homepage, landing pa |
| `gpt-image-2` | [`02-content-social/gpt-image-2`](./02-content-social/gpt-image-2) | Generate images with OpenAI GPT Image 2 (model id `gpt-image-2`) — Charles's default image generator on Hermes |

## Maintenance Rules

- Keep `SKILL.md` focused on when to use the skill and how to operate it.
- Keep API keys, tokens, host passwords, and private environment values out of git.
- Do not re-add system/default skills removed by the client cleanup pass.

## License

Private collection for Mad Scientist systems and related agent workflows.
