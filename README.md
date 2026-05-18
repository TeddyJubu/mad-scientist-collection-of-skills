# Mad-Agent Skills Library

A complete, organized library of AI skills powering Charles Blair's REI business automation system — Hermes Gateway + OpenClaw.

## Structure

```
Mad-agent-skills/
├── 01-real-estate/          # Property research, skip tracing, rehab estimation
├── 02-content-social/       # YouTube, thumbnails, social posting, content repurposing
├── 03-productivity/         # Notion, email, file delivery, documents, PDF generation
├── 04-devops-infrastructure/ # Docker, Traefik, Vercel, systemd, port management
├── 05-data-research/        # Apify, Apollo, Census, Melissa, Brave Search, SEO
├── 06-ai-agents/            # Bob, Sarah, HR, OpenClaw management, whisper, browser
├── 07-image-graphics/       # AI image gen, thumbnails, HeyGen, Remotion, graphic design
├── 08-communication/         # Discord, video meetings, Zoom processor
├── 09-media-lifestyle/       # Weather, health, audio TTS, Spotify, video frames
├── 10-openclaw-mcp/         # OpenClaw platform skills + MCP client
├── 11-software-development/  # Code review, debugging, TDD, planning, CI/CD
└── 12-tools/                # Catch-all: mlops, gaming, feeds, smart-home, etc.
```

## Category Details

### 01 — Real Estate
| Skill | What it does |
|---|---|
| `batchdata-skip-trace` | Batch property owner lookup via BatchData API |
| `homedepot-repair-estimator` | Room-by-room rehab cost estimate from photos |
| `landglide-lookup` | US parcel data lookup via LandGlide/ReportAll |
| `mad-skip-trace` | Skip trace by property address |
| `owner-skip-trace` | Owner lookup by name + address |
| `rentcast-property-report` | Full investment analysis from RentCast |
| `sdat-property-search` | Maryland property records (SDAT) |

### 02 — Content & Social
| Skill | What it does |
|---|---|
| `copywriting` | REI-focused marketing copy generation |
| `gpt-image-2` | OpenAI GPT Image 2 generation (default) |
| `yt-thumbnail-creator` | YouTube thumbnails (MrBeast style) |
| `instagram-carousel-authority` | Viral authority-building carousels |
| `content-repurposing-engine` | Turn one content piece into 10+ formats |
| `blotato-text-poster` | Post text to FB, YT, IG, LI, TT, X |
| `xitter` | X/Twitter via xurl CLI |
| `youtube-opus-skill` | OpusClip video clipping pipeline |
| `supadata-transcript` | YouTube/TikTok/Twitter/IG transcript extraction |
| `nova-youtube-agent` | YouTube automation agent |
| `opus-clip-mcp` | Send videos to OpusClip via Zapier MCP |
| `opus-blotato-video-poster` | Clip → post to Blotato (all platforms) |
| `video-transcribe-and-timestamp` | Transcribe + timestamp video files |
| `mad-graphic-designer-skill` | Real estate team graphic design |
| `Content Repurposer` | Multi-format content transformation |

### 03 — Productivity
| Skill | What it does |
|---|---|
| `notion-cli` | Notion API via curl (preferred over ntn CLI) |
| `notion-mastery` | Advanced Notion workflows |
| `notion-beautiful-systems` | Polished Notion page design system |
| `agentmail` | Dedicated email inbox via AgentMail |
| `himalaya` | IMAP/SMTP email from terminal |
| `gmail-unread-autodraft` | Scan Gmail → auto-draft replies |
| `gog` | Google Workspace (Gmail, Calendar, Drive, Contacts) |
| `airtable` | Airtable REST API via curl |
| `google-workspace` | Gmail, Calendar, Drive, Sheets, Docs |
| `powerpoint` | Create/edit .pptx decks |
| `ocr-and-documents` | Extract text from PDFs/scans |
| `nano-pdf` | Edit PDF text/typos/titles via CLI |
| `maps` | Geocode, POIs, routes via OpenStreetMap |
| `linear` | Linear issues/projects via GraphQL |
| `teams-meeting-pipeline` | Teams meeting summary pipeline |
| `pdf-generation` | Generate PDFs (fpdf2 fallback) |
| `file-delivery` | Hermes → Telegram file delivery |
| `filebrowser-deploy` | Web file manager behind Traefik |
| `obsidian` | Obsidian vault read/write/search |

### 04 — DevOps & Infrastructure
| Skill | What it does |
|---|---|
| `docker-management` | Containers, images, volumes, networks |
| `kanban-orchestrator` | Decomposition playbook + anti-temptation rules |
| `kanban-worker` | Kanban execution pitfalls/examples |
| `service-deployment-and-monitoring` | Deploy + auto-heal + port management |
| `traefik-docker-deploy` | Docker apps behind Traefik reverse proxy |
| `systemd-port-reservation` | Lock ports to long-running services |
| `vercel-deploy` | Next.js app deployment to Vercel |
| `vercel-site-deploy` | Static HTML site → Vercel |
| `lb-vercel-skill` | Vercel CLI management |
| `vercel-runner` | Vercel project operations |

### 05 — Data & Research
| Skill | What it does |
|---|---|
| `apify-actor-finder` | Search Apify store for actors |
| `apify-runner` | Run Apify actors with token management |
| `apify-mcp` | MCP server for Apify (mcpc @apify) |
| `brave-search` | Brave Search API + content extraction |
| `census-data` | US Census Bureau demographic data |
| `melissa-data-information` | Melissa Data property/ownership lookup |
| `apollo-find` | Apollo.io B2B people/company search |
| `firecrawl` | Scrape/crawl websites to clean markdown |
| `firehose` | Real-time web monitoring via Firehose API |
| `mad-census-baby` | Census data via Mad Scientist wrapper |
| `seo-audit` | SEO review/diagnosis for websites |
| `research` | arxiv, blogwatcher, llm-wiki, polymarket |

### 06 — AI & Agents
| Skill | What it does |
|---|---|
| `bob` | BatchData skip-trace + general ops |
| `sarah-outbound-caller` | VAPI AI voice calling agent |
| `hr` | HR intelligence system for founders |
| `hr-hiring` | Upwork job post + candidate screening |
| `beautiful-websites` | Find businesses with outdated sites → redesign |
| `openclaw-access-troubleshooting` | OpenClaw access/troubleshooting |
| `openclaw-agent-creation` | Create new OpenClaw subagent workspace |
| `openclaw-docker-migration` | Migrate OpenClaw from Docker to Hermes |
| `openclaw-platform-management` | OpenClaw platform operations |
| `autonomous-ai-agents` | Spawn autonomous AI coding agents |
| `openai-whisper-api` | OpenAI Whisper transcription |
| `openclaw-agent-browser` | Headless browser automation for OpenClaw |
| `openclaw-logo-maker` | Logo generation for OpenClaw agents |
| `agent-browser` | Rust headless browser automation CLI |
| `mcporter` | MCP client CLI (list, configure, call) |
| `pikastream-video-meeting` | Join Google Meet/Zoom as AI agent |
| `rei-ai-zoom-processor` | Zoom transcript → summary + content |
| `enhancor` | Enhancor API integration |

### 07 — Image & Graphics
| Skill | What it does |
|---|---|
| `gpt-image-2` | OpenAI GPT Image 2 (default image gen) |
| `gemini-image-editor` | Edit existing images (background swap, remove objects) |
| `nano-banana-pro` | Gemini 3 Pro image generation |
| `nano-banana-image-gen` | Gemini 3.1 Flash image generation |
| `graphic-design` | From basic visuals to professional designs |
| `superdesign` | 54 real design systems as HTML/CSS reference |
| `heygen-avatar-video` | AI avatar videos via HeyGen API |
| `remotion` | Programmatic video creation with React |
| `veed_fabtoc_1.0` | Talking video from user-provided image |
| `pixel-art` | Pixel art with era palettes (NES, Game Boy) |
| `ascii-art` | ASCII art, cowsay, boxes |
| `architecture-diagram` | Dark-themed SVG architecture/cloud diagrams |

### 08 — Communication
| Skill | What it does |
|---|---|
| `discord` | Control Discord via Clawdbot |

### 09 — Media & Lifestyle
| Skill | What it does |
|---|---|
| `claude-video` | Watch/analyze any video URL |
| `fish-audio-tts` | Fish Audio TTS generation |
| `gif-search` | Tenor GIF search/download |
| `healthcheck` | Track water and sleep |
| `heartmula` | Suno-like song generation |
| `songsee` | Audio spectrogram/feature extraction |
| `spotify` | Spotify play, search, queue, playlists |
| `video-frames` | Extract frames/clips from videos |
| `weather` | Current weather + forecasts (no API key) |
| `youtube-content` | YouTube transcript fetch + transform |

### 10 — OpenClaw & MCP
| Skill | What it does |
|---|---|
| `openclaw` | OpenClaw platform management |
| `mcp` | MCP client (native + mcporter bridge) |

### 11 — Software Development
| Skill | What it does |
|---|---|
| `software-development` | Code review, debugging, TDD, planning, CI/CD |

### 12 — Tools
| Skill | What it does |
|---|---|
| `apple` | macOS/iCloud integrations (Reminders, FindMy, Notes, iMessage) |
| `browser-use-cloud` | Browser Use Cloud API (managed AI browser) |
| `creative` | ASCII art, diagrams, p5.js, songwriting |
| `daily-eod-report` | Daily end-of-day agent report |
| `data-science` | Jupyter live kernel, pandas, visualization |
| `devops` | Docker, kanban, service deployment |
| `diagramming` | Excalidraw JSON diagrams |
| `dogfood` | Exploratory QA testing of web apps |
| `domain` | Domain management |
| `email` | Email workflows |
| `feeds` | RSS/Atom feed monitoring |
| `gaming` | Minecraft, Pokemon via headless emulator |
| `gifs` | GIF search and management |
| `github` | GitHub PR, issues, repos, code review |
| `gohighlevel-api` | GoHighLevel CRM API |
| `google-drive-image-upload` | Auto-upload images to Google Drive |
| `inference-sh` | Model serving, quantization, vLLM |
| `leisure` | Find nearby restaurants, cafes, bars |
| `mad-event-maker` | High-converting REI event copy |
| `mlops` | HuggingFace, Weights & Biases, lm-eval |
| `note-taking` | Note taking and research collaboration |
| `productivity` | Document creation, spreadsheets, presentations |
| `real-estate` | Property contact research |
| `red-teaming` | LLM jailbreaks (GODMODE, etc.) |
| `rei-ai-weekly-newsletter` | Weekly REI newsletter generation |
| `remotion-video-editing` | Remotion video editing |
| `service-health-monitoring` | Auto-healing cron monitoring |
| `skill-to-web-app` | Wrap Hermes skill as public website |
| `smart-home` | Philips Hue lights/home automation |
| `social-media` | Xitter, blotato, social posting |
| `yuanbao` | Yuanbao groups (@mention, query info) |

---

## Setup

### API Keys
Some skills require API keys stored in `.env` files. Never commit `.env` files.
```
~/.hermes/skills/<skill>/.env        # skill-level key
~/.hermes/.env                       # host-level keys (Notion, etc.)
```

### Skill Format
Each skill lives in its own folder:
```
<skill>/
├── SKILL.md           # Main skill definition
├── scripts/           # Helper scripts
├── references/        # API docs, examples, guides
├── assets/            # Images, data files
└── .env                # API keys (gitignored)
```

## License
Private — Charles Blair / Mad Scientist REI Systems
