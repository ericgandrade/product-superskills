# 📦 Product Superskills v1.0.0

8 AI skills for product management, strategy, GTM, and startup growth. A composable Modern Product Operating Model — install once across all 8 AI platforms.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Skills](https://img.shields.io/badge/skills-8-brightgreen.svg)
![Platforms](https://img.shields.io/badge/platforms-8-orange.svg)

## 🚀 Quick Install

**One-liner (recommended):**
```bash
curl -fsSL https://raw.githubusercontent.com/ericgandrade/product-superskills/main/scripts/install.sh | bash
```

**Or use NPX (zero-install):**
```bash
npx product-superskills
```

The installer detects and installs to all 8 AI platforms on your machine: Claude Code, GitHub Copilot, OpenAI Codex, OpenCode, Gemini CLI, Antigravity, Cursor IDE, AdaL CLI.

**Other methods:**
```bash
# npm global
npm install -g product-superskills

# With bundles
npx product-superskills --bundle core-product -y
npx product-superskills --bundle growth -y
```

**Local install (no npm/npx required):**
```bash
git clone https://github.com/ericgandrade/product-superskills
cd product-superskills

./scripts/local-install.sh        # Interactive
./scripts/local-install.sh -y     # Auto-install to all detected platforms
./scripts/local-install.sh -y -q  # Silent (CI / scripted)
```

**Uninstall:**
```bash
curl -fsSL https://raw.githubusercontent.com/ericgandrade/product-superskills/main/scripts/uninstall.sh | bash
```

## 🔌 Claude Code Plugin (Native)

Requires **Claude Code v1.0.33+** (`claude --version` to check).

**Method 1: Interactive UI (Inside a running `claude` session) — Recommended**

```text
/plugin marketplace add ericgandrade/product-superskills
/plugin install product-superskills@product-superskills
```

**Method 2: Local test (no install needed)**

```bash
git clone https://github.com/ericgandrade/product-superskills
claude --plugin-dir ./product-superskills
```

### Once installed — all 8 skills under the `product-superskills:` namespace

```
/product-superskills:product-operating-model
/product-superskills:product-strategy
/product-superskills:product-discovery
/product-superskills:product-architecture
/product-superskills:product-delivery
/product-superskills:product-leadership
/product-superskills:abx-strategy
/product-superskills:startup-growth-strategist
```

## ✨ Features

- **8 Product & Strategy Skills** - Full Modern Product Operating Model
- **Zero-Config Install** - Run once, works everywhere
- **Curated Bundles** - Core PM, Architecture, Growth & GTM
- **8 Platform Support** - GitHub Copilot, Claude Code, Codex, OpenCode, Gemini, Antigravity, Cursor, AdaL
- **No API Keys Required** - All skills run natively in your AI tool

## 📦 Available Skills

### 🗺️ Modern Product Operating Model
| Skill | Version | Purpose |
|-------|---------|---------|
| **product-operating-model** | v2.0.0 | Index and entry point for the Modern Product Operating Model — 6 composable skills covering strategy, discovery, architecture, delivery, AI-native development, and leadership |
| **product-strategy** | v2.0.0 | Build product strategy that drives real choices — where to play, how to win, ICP, positioning, pricing, GTM, and strategic bets |
| **product-discovery** | v2.0.0 | Run continuous discovery using OSTs, weekly interview rhythm, assumption testing, and Opportunity Solution Trees to find problems worth solving |
| **product-architecture** | v2.0.0 | Convert discovery opportunities into prioritized bets and roadmaps — capability blocks, solution briefs, and quarterly cycles without false precision |
| **product-delivery** | v2.0.0 | Ship, measure, and learn with staged rollouts, metrics hierarchies, bet retrospectives, and GTM launch execution |
| **product-leadership** | v2.0.0 | Operate as Director or CPO — portfolio management, executive alignment, board communication, team structure design, and operating rhythms |

### 🚀 Growth & GTM
| Skill | Version | Purpose |
|-------|---------|---------|
| **abx-strategy** | v2.1.0 | Build Account-Based Everything (ABX) GTM strategies for complex B2B sales — ICP scoring, messaging architecture, and pipeline acceleration for $100K+ deals with 6+ month cycles |
| **startup-growth-strategist** | v2.0.0 | Validate a business idea, calculate TAM/SAM/SOM, project financial growth, and design a Go-To-Market strategy — market sizing, unit economics, and competitive analysis in one unified workflow |

## 🎯 Curated Bundles

```bash
# Core Product Management (5 skills)
npx product-superskills --bundle core-product -y

# Product Architecture only
npx product-superskills --bundle architecture -y

# Growth & GTM (2 skills)
npx product-superskills --bundle growth -y

# All Product Skills (complete collection)
npx product-superskills --bundle all -y
```

## 🚀 Quick Start Examples

```bash
# Run a full product strategy session
claude -p "build a product strategy for our B2B SaaS — we target mid-market HR teams"

# Set up continuous discovery
claude -p "help me design a weekly discovery rhythm for my product team"

# Design an ABX GTM motion
claude -p "build an ABX strategy for our enterprise pipeline — $200K ACV, 9-month sales cycle"

# Calculate market size for a new idea
claude -p "size the market for an AI-powered fleet management tool"
```

## 💻 Supported Platforms

- **GitHub Copilot CLI** - Terminal AI assistant (`~/.github/skills/`)
- **Claude Code** - Anthropic's Claude in development (`~/.claude/skills/`)
- **OpenAI Codex** - GPT-powered coding assistant (`~/.codex/skills/`)
- **OpenCode** - Open source AI coding assistant (`~/.agent/skills/`)
- **Gemini CLI** - Google's Gemini in terminal (`~/.gemini/skills/`)
- **Antigravity** - AI coding assistant (`~/.gemini/antigravity/skills/`)
- **Cursor IDE** - AI-powered code editor (`~/.cursor/skills/`)
- **AdaL CLI** - AI development assistant (`~/.adal/skills/`)

## ⌨️ Compatibility & Invocation

| Tool | Type | Invocation Example | Path |
|------|------|--------------------|------|
| **Claude Code** | CLI | `/product-strategy help me...` | `~/.claude/skills/` |
| **Gemini CLI** | CLI | `Use product-discovery to...` | `~/.gemini/skills/` |
| **Codex CLI** | CLI | `Use abx-strategy to...` | `~/.codex/skills/` |
| **Antigravity** | IDE | *(Agent Mode)* `Use skill...` | `~/.gemini/antigravity/skills/` |
| **Cursor** | IDE | `@startup-growth-strategist` in Chat | `~/.cursor/skills/` |
| **Copilot** | Ext | *(Paste skill content manually)* | N/A |
| **OpenCode** | CLI | `opencode run @product-leadership` | `~/.agent/skills/` |
| **AdaL CLI** | CLI | *(Auto)* Skills load on-demand | `~/.adal/skills/` |

## ⚡ CLI Commands & Shortcuts

| Command | Shortcut | Purpose |
|---------|----------|---------|
| `install` | `i` | Install skills |
| `list` | `ls` | List installed skills |
| `status` | `st` | Show global install status + version differences |
| `update` | `up` | Smart update (outdated + missing skills) |
| `uninstall` | `rm` | Remove skills |
| `doctor` | `doc` | Check installation |

```bash
npx product-superskills i -a -y -q    # Install all, skip prompts, quiet mode
npx product-superskills status         # Show global status + skill version differences
npx product-superskills up -y          # Update outdated + install missing skills
npx product-superskills ls -q          # List with minimal output
npx product-superskills --list-bundles # Show available bundles
```

## 📋 System Requirements

- Node.js 14+ (for installer)
- One or more supported platforms installed

## 🔒 Privacy

product-superskills does not collect, store, transmit, or share any user data.

- **No external servers** — no backend, no telemetry, no network requests of its own
- **No API keys required** — all skills run within your AI tool using native tools
- **No logging** — nothing is recorded outside of your local session
- **Open source** — all skill logic is fully auditable

## 📄 License

MIT - See [LICENSE](./LICENSE) for details.

## 🔗 Quick Links

- 📝 [Changelog](CHANGELOG.md) - Release history
- 🐛 [Issues](https://github.com/ericgandrade/product-superskills/issues) - Report problems

## Part of the Superskills Family

| Package | Skills | Focus | Install |
|---------|--------|-------|---------|
| [claude-superskills](https://github.com/ericgandrade/claude-superskills) | 18 | Core: orchestration, planning, research & content | `npx claude-superskills` |
| [obsidian-superskills](https://github.com/ericgandrade/obsidian-superskills) | 6 | Obsidian knowledge management | `npx obsidian-superskills` |
| [career-superskills](https://github.com/ericgandrade/career-superskills) | 20 | Job search & career development | `npx career-superskills` |
| **product-superskills** | 8 | Product management & GTM strategy | `npx product-superskills` |
| [design-superskills](https://github.com/ericgandrade/design-superskills) | 9 | UI/UX design, brand & diagrams | `npx design-superskills` |
| [avanade-superskills](https://github.com/ericgandrade/avanade-superskills) | 3 | Avanade-branded content (private) | `git clone git@github.com:ericgandrade/avanade-superskills.git` |

---

**Built with ❤️ by [Eric Andrade](https://github.com/ericgandrade)**

*Version 1.0.0 | May 2026*
