# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

This is **not a software project** — there is no build, lint, test, or runtime. It is the **Yard Mastery Design System**: a structured, machine-readable knowledge base that an AI graphic designer ("Claude Design") reads to generate on-brand emails, social posts, and AI images. The "source code" is Markdown rules + reusable templates/prompts, plus a single `brand-board.html` visual summary (open directly in a browser).

Your two modes of work here are: (1) **generating content** using the system, and (2) **maintaining/extending** the system itself.

## Architecture: how the files relate

Everything is indexed by `README.md`, which is the entry point. The system is deliberately modular so a content task loads only the relevant files rather than all of them:

- `guidelines/` — the authoritative brand rules, numbered `01`–`06` (foundation/voice → visual identity → imagery → products → layout & channels → copywriting). These are the source of truth.
- `prompts/` — `image-prompt-library.md` (ready-made AI image prompts by use case) composed with `style-tokens.md` (reusable fragments: BASE_STYLE, COLOR_DIRECTION, LIGHTING, LENS, COMPOSITION, negatives). Image generation = subject from the library + tokens.
- `templates/` — fill-in-the-blank email/social skeletons.
- `assets/` — binary files + `ASSET-LOG.md` registry. `generated/` is where new assets Claude creates go.

**File-loading map for a content task** (from README): always load `guidelines/01` (voice) + `02` (visual identity); then add `05`+`06`+`templates/email-templates.md` for email, `05`+`templates/social-templates.md` for social, or `prompts/*`+`guidelines/03` for images. Product content always loads `guidelines/04`.

## Non-negotiable rules when generating content

- **Never invent product names, NPK numbers, claims, coverage, or prices.** Always pull them from `guidelines/04-products.md`. When in doubt, check the live site (yardmastery.com) or ask.
- Brand voice is a "confident coach": plain-spoken, encouraging, expert, talks to "you."
- Core tokens (defined in `02-visual-identity.md`): green `#64B356`, gold `#E0C030`, action green `#02AE65`, sale red `#D12442`, ink `#191919`; type Roboto (headlines) + Lora (body).
- Run output against the do/don't lists and the pre-flight checklist in `guidelines/05-layout-and-channels.md` before considering it done.

## Conventions when extending the system

- **New asset created** → save to `assets/generated/` using the naming rule `YYYY-MM-DD_channel_campaign-or-subject_variant.ext` (lowercase, hyphen-separated; channel ∈ email/ig/fb/yt/x/story/print; include aspect ratio or pixel size), then **add a row to `assets/ASSET-LOG.md`** (newest at top).
- **New brand rule/pattern** → edit the relevant `guidelines/` file; keep the existing format (rule + concrete Do / Don't example).
- **New reusable prompt/fragment** → `prompts/image-prompt-library.md` and/or `prompts/style-tokens.md`.
- **Any change** → add a dated line to `CHANGELOG.md` (format `## YYYY-MM-DD — short summary`, newest above the trailing HTML comment).
- Formatting house style: Markdown headings for scannability, hex codes in backticks, every guideline paired with a Do/Don't where possible, product facts always cite the catalog.

## Known state

- The Shopify store connector is **not yet authenticated**. Until it is, product data in `04-products.md` is sourced from the live site, not auto-synced. (A Shopify MCP server is available in this environment if/when connecting it becomes the task.)
- Logo white/knockout variants are not yet in `assets/logo/`.
