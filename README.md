# 🐶 Fulai (福来) Content Pipeline

> *"All good lucks come home"* ✨

Automated content research & scripting pipeline for Fulai's social media channel.

## Architecture

```
puppy-content/
├── config.md              # Fulai's profile + content strategy
├── README.md              # This file
├── archive/               # Daily story briefs (auto-generated)
│   └── story-brief-YYYY-MM-DD.md
├── scripts/               # Future: video scripts
├── templates/             # Content templates
│   ├── story-brief.md     # Template for daily trending research
│   └── video-script.md    # Template for 30-60s video scripts
└── assets/                # Media assets (Fulai photos, branding)
```

## Pipeline

```
🌅 8:00 AM SGT — Daily Trending Search (cron)
    └─ Searches 8+ queries for viral dog content
    └─ Writes story-brief-YYYY-MM-DD.md to archive/
    └─ Suggests Fulai-specific angles for each story
    └─ Includes Mom-Cam filming requests
    └─ Delivers summary to Telegram
```

## Platforms

| Platform | Priority | Content Type |
|---|---|---|
| TikTok | Primary | 30-60s vertical videos |
| Xiaohongshu (RED) | Secondary | Chinese-market videos |
| Instagram Reels | Cross-post | Same content, format tweaks |

## Content Pillars

1. **Daily Luck** 🍀 — Fulai's "lucky" moments
2. **Trending Reactions** 📖 — Reacting to viral dog stories
3. **Mom-Cam Footage** 📹 — Raw clips edited with storytelling
4. **7 Years Wisdom** 🎂 — "What my dog taught me" moments
5. **Mixed Breed Pride** 🐕 — Celebrating uniqueness

## Cron Jobs

- `puppy-content-trending-search` — Daily 8am SGT, searches trending dog stories

## Quick Start

Ask Rinちゃん: "What's trending for Fulai today?" — reads the latest story brief.

---

*Managed by Rinちゃん ✨⚡️🌟☀️*
