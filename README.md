<p align="center">
  <img src="https://foxl.ai/favicon.svg" width="96" alt="Foxl" />
</p>

<h1 align="center">Foxl</h1>

<p align="center">
  <a href="https://foxl.ai"><img src="https://img.shields.io/badge/Website-foxl.ai-0b5ed7?style=for-the-badge" alt="Website"></a>
  <a href="https://app.foxl.ai"><img src="https://img.shields.io/badge/Web%20App-app.foxl.ai-0b5ed7?style=for-the-badge" alt="Web App"></a>
  <a href="https://docs.foxl.ai"><img src="https://img.shields.io/badge/Docs-docs.foxl.ai-FFD700?style=for-the-badge" alt="Docs"></a>
  <a href="https://discord.gg/6J53VyV2Fy"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord"></a>
  <a href="https://github.com/foxl-ai/foxl/releases/latest"><img src="https://img.shields.io/github/v/release/foxl-ai/foxl?label=Download&style=for-the-badge&color=16a34a" alt="Download"></a>
</p>

---

**Your 24/7 personal AI agent — on your desktop, in your browser, and in your pocket.**

Foxl is a personal AI agent that actually does things for you. It drives your real Chrome browser (with your logins intact), writes and runs code in a sandboxed workspace, manages files, spawns subagents in parallel, and runs schedules around the clock. It ships as a signed desktop app for macOS and Windows, a web app at [app.foxl.ai](https://app.foxl.ai), and a Chrome extension. Talk to it from your laptop, then keep the conversation going from Slack, Discord, or a browser tab.

Powered by Claude Opus 4.7 and Sonnet 4.6 by default, with optional BYOK for Anthropic, OpenAI, Google Gemini, local Ollama, and your Claude Pro/Max or ChatGPT Plus subscription via OAuth. Switch models mid-conversation — no reconfiguration, no lock-in.

<table>
<tr><td><b>A real browser, not a headless clone</b></td><td>Controls your actual Chrome with all your logged-in sessions, cookies, and extensions. No re-authentication, no bot detection, no brittle scraping.</td></tr>
<tr><td><b>Multi-agent orchestration</b></td><td>Spawn up to 5 concurrent subagents for parallel research, coding, and analysis. Auto-continuation synthesizes results when workers finish — no manual wrangling.</td></tr>
<tr><td><b>Runs 24/7 in the background</b></td><td>Native menubar / system tray app. Schedules, heartbeats, and webhooks keep Foxl working while your laptop sleeps. Daily reports, nightly backups, weekly audits — all in natural language.</td></tr>
<tr><td><b>Persistent memory across sessions</b></td><td>File-backed memory that Foxl curates itself — user profile, feedback, project state, external references. Durable across updates, searchable, human-editable.</td></tr>
<tr><td><b>Skill library</b></td><td>Curated skills for messaging, productivity, media, browser automation, development workflows, and more. One-click install, auto-sync with the Foxl skills repo, fully local.</td></tr>
<tr><td><b>Adaptive thinking</b></td><td>Claude Opus 4.7 / Sonnet 4.6 adaptive extended thinking scales reasoning effort to the task — cheap for lookups, deep for planning and debugging.</td></tr>
<tr><td><b>Local-first, private by default</b></td><td>Conversations, credentials, files, and skills live on your machine. BYOK keys never leave your laptop. Relay is optional for metered access on the go.</td></tr>
<tr><td><b>Cross-device, cross-surface</b></td><td>Desktop (macOS + Windows), web (app.foxl.ai), Chrome extension (for in-page agent actions), and a tunneled relay so you can reach your home agent from your phone.</td></tr>
</table>

## Download

| Platform | Installer | Requirements |
|----------|-----------|--------------|
| **macOS** (Universal, arm64 + x64) | [Foxl-latest-universal.dmg](https://github.com/foxl-ai/foxl/releases/latest/download/Foxl-latest-universal.dmg) | macOS 12 Monterey or later, Apple Silicon & Intel |
| **Windows** (Installer) | [Foxl-latest-setup.exe](https://github.com/foxl-ai/foxl/releases/latest/download/Foxl-latest-setup.exe) | Windows 10 or later, x64 |
| **Windows** (Portable) | [Foxl-latest-portable.zip](https://github.com/foxl-ai/foxl/releases/latest/download/Foxl-latest-portable.zip) | Windows 10 or later, no install needed |
| **Chrome Extension** | [Chrome Web Store](https://foxl.ai#download) | Chrome / Edge / Brave |
| **Web App** | [app.foxl.ai](https://app.foxl.ai) | Any modern browser |

macOS and Windows builds are signed and ship with auto-update (Squirrel / electron-updater). Code-signed Windows builds currently use a self-signed certificate — SmartScreen may prompt on first launch. See the [install guide](https://docs.foxl.ai/install) for signing details and enterprise rollout tips.

## Quick Start

After install, launch Foxl. The first-run wizard walks you through:

1. **Sign in** — with Google, Apple, or email magic link (optional; local-only mode works without an account)
2. **Connect a model** — default Claude via Foxl relay (credits included), or BYOK your own Anthropic / OpenAI / Google / Ollama endpoint
3. **Authorize browser control** — Foxl launches your existing Chrome profile; no separate login needed
4. **Pick a starting skill** — morning briefing, research assistant, code reviewer, or start empty

Then just talk. Foxl figures out whether it needs the browser, the terminal, a subagent, or just to think.

## Plans

| Plan | Price | Credits | Models |
|------|-------|---------|--------|
| **Free** | $0 | 10 credits / month | Claude Sonnet 4.6, Haiku 4.5 |
| **Pro** | $20 / month | 500 credits / month | All models including Opus 4.7 |
| **Ultra** | $200 / month | 10,000 credits / month | All models, priority routing |
| **BYOK** | Free on every plan | Uses your API keys | Anthropic, OpenAI, Google, Ollama, Claude Pro/Max, ChatGPT Plus |

Every account also gets **200 welcome credits** that never expire. See [foxl.ai/#pricing](https://foxl.ai/#pricing).

## Messaging & Integrations

Foxl reaches you wherever you already work:

- **Browser extension** — in-page agent actions, content capture, multi-tab coordination
- **Chrome DevTools** — agent-driven debugging with full page context
- **Gateway channels** (beta) — Discord, Slack, Telegram bridges run off the same Foxl relay
- **Webhooks & cron** — every schedule can trigger Discord, email, or a custom webhook

## Documentation

Full docs at [docs.foxl.ai](https://docs.foxl.ai):

| Section | Covers |
|---------|--------|
| [Quickstart](https://docs.foxl.ai/quickstart) | Install → sign in → first conversation |
| [Models](https://docs.foxl.ai/models) | Opus 4.7, Sonnet 4.6, Haiku 4.5, adaptive thinking |
| [Providers](https://docs.foxl.ai/providers) | BYOK setup, Claude Code OAuth, OpenAI OAuth, Ollama |
| [Tools](https://docs.foxl.ai/tools) | Browser, code, exec, files, git, memory, scheduling |
| [Skills](https://docs.foxl.ai/skills) | Installing skills, skill sync, writing your own |
| [Conversations](https://docs.foxl.ai/conversations) | Thread model, extended thinking, context management |
| [Web App](https://docs.foxl.ai/web-app) | app.foxl.ai features, sign-in, cross-device sync |
| [Schedules](https://docs.foxl.ai/schedules) | Cron, heartbeat, webhook-triggered automations |
| [Credits](https://docs.foxl.ai/credits) | Per-model pricing, top-ups, BYOK cost model |
| [FAQ](https://docs.foxl.ai/faq) | Common questions, troubleshooting, security |

## Community

- **Discord** — [discord.gg/6J53VyV2Fy](https://discord.gg/6J53VyV2Fy) — questions, feedback, announcements
- **Issues** — [github.com/foxl-ai/foxl/issues](https://github.com/foxl-ai/foxl/issues) — bug reports and feature requests
- **Changelog** — [foxl.ai/#changelog](https://foxl.ai/#changelog) — every release, every fix
- **Blog** — [foxl.ai/blog](https://foxl.ai/blog) — engineering deep-dives, release notes, product stories

## Security

Found a security issue? Email [security@foxl.ai](mailto:security@foxl.ai) or open a [private security advisory](https://github.com/foxl-ai/foxl/security/advisories/new). Foxl signs macOS builds with a Developer ID certificate, code-signs Windows binaries, and ships with source-map stripping in release artifacts. See [docs.foxl.ai/security](https://docs.foxl.ai/security) for the full threat model.

## License

Foxl is proprietary software — see [LICENSE](LICENSE). This repository distributes signed release binaries only; the agent runtime, relay, and web apps are developed in a private monorepo.

---

<p align="center">
  Built by <a href="https://foxl.ai">Foxl AI</a> · <a href="https://foxl.ai">foxl.ai</a>
</p>
