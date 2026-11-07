# App Store Optimization (ASO) Audit Skill

[![skills.sh](https://skills.sh/b/tudorturcanu/aso-skill)](https://skills.sh/tudorturcanu/aso-skill)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Compatible-orange.svg)](https://anthropic.com)
[![Google Antigravity](https://img.shields.io/badge/Antigravity-Compatible-blue.svg)](https://deepmind.google)
[![License: MIT](https://img.shields.io/badge/license-MIT-purple.svg)](LICENSE)

An agent skill that equips your AI coding assistant (Claude Code, Google Antigravity, Cursor, Codex, etc.) to perform comprehensive **App Store Optimization (ASO)** audits on **Apple App Store** and **Google Play Store** listings.

Fetches live listing data, scores the app across 6 core dimensions, benchmarks against category leaders, and generates prioritized, concrete action plans.

---

## Install

Install globally across all projects:

```bash
npx skills add tudorturcanu/aso-skill -g
```

Or install for your current project directory:

```bash
npx skills add tudorturcanu/aso-skill
```

---

## When to Use

Trigger the skill whenever you provide an App Store or Google Play link or ask for store visibility advice:

> "Here's our App Store link: https://apps.apple.com/us/app/my-app/id123456789. Audit our listing and show what to improve."
> "How can we optimize our Google Play store page to improve conversion and search ranking?"
> "Review our app listing screenshots and subtitle for better keyword targeting."

---

## What the Skill Does

- **Multi-Store Intelligence:** Automatically parses and differentiates Apple App Store rules (30-char titles, 30-char subtitles, 170-char promo text, hidden keyword fields) from Google Play Store rules (30-char titles, 80-char short descriptions, 4,000-char indexed descriptions, feature graphics).
- **Brand Maturity Calibration:** Calibrates expectations based on brand tier (Dominant, Established, Challenger) so emerging startups get actionable growth keywords rather than generic enterprise advice.
- **6-Dimension Scoring System (0–100):**
  1. Title & Subtitle / Short Description (20%)
  2. Long Description & Keyword Density (15%)
  3. Visual Assets & Screenshots (25%)
  4. Ratings, Volume & Reviews Sentiment (20%)
  5. Metadata & Release Cadence Freshness (10%)
  6. Conversion Signals & Badges (10%)
- **Actionable Copy Recommendations:** Generates precise `change "X" to "Y"` copy suggestions with exact character counts to maximize indexing and tap-through rates without exceeding store limits.
- **Top 3 Quick Wins:** Surfaces immediate high-impact changes alongside long-term conversion recommendations.

---

## Repository Layout

```
skills/aso/
├── SKILL.md                          # Core audit instructions and phased workflow
├── evals/
│   └── evals.json                    # Benchmark evaluation prompts and assertions
└── references/
    ├── apple-specs.md                # App Store Connect character limits and asset specs
    ├── benchmarks.md                 # Category benchmark data across store verticals
    ├── google-play-specs.md          # Google Play Console asset specifications
    ├── report-template.md            # Markdown report scorecard template
    └── scoring-criteria.md           # Rubric for scoring each dimension
```

---

## License

[MIT](LICENSE) © 2026 Tudor Turcanu
