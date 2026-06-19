# Yard Mastery Design System

**The single source of truth for the Yard Mastery brand — built for "Claude Design" (our AI graphic designer) to generate on-brand emails, social posts, and images.**

This system turns Yard Mastery's brand into clear, machine-readable rules and reusable building blocks. If you are Claude Design (or any teammate making content), **read this file first**, then load only the sections you need for the task at hand.

---

## How to use this system (Claude Design, start here)

Before generating anything, load the files relevant to your task:

| If you're making… | Load these files |
|---|---|
| Any content (always) | `guidelines/01-brand-foundation.md` (voice) + `guidelines/02-visual-identity.md` (color/type/logo) |
| A marketing **email** | `guidelines/05-layout-and-channels.md` + `guidelines/06-copywriting.md` + `templates/email-templates.md` |
| A **social post** (IG/FB/YT/X) | `guidelines/05-layout-and-channels.md` + `templates/social-templates.md` |
| An **AI-generated image** | `prompts/image-prompt-library.md` + `prompts/style-tokens.md` + `guidelines/03-imagery.md` |
| **Product** content | `guidelines/04-products.md` (names, NPK, claims, coverage) |

**The golden rule:** never invent product names, NPK numbers, claims, or prices. Pull them from `guidelines/04-products.md`. When in doubt, ask or check the live site.

### A reliable workflow for any request
1. **Clarify** the brief: channel, goal, audience (warm- vs cool-season lawn?), season, product(s), offer, deadline.
2. **Load** the relevant files above.
3. **Draft** copy using `06-copywriting.md` formulas and approved vocabulary.
4. **Compose** the visual using `02-visual-identity.md` (color/type) + `03-imagery.md` (look) or the `prompts/` library for AI images.
5. **Check** against the do/don't lists and the pre-flight checklist in `guidelines/05-layout-and-channels.md`.
6. **Save & log** any new asset to `assets/generated/` and add a row to `assets/ASSET-LOG.md`.

---

## What's in here

```
ym-design-system/
├── README.md                      ← you are here (index + how-to + how-to-extend)
├── CHANGELOG.md                   ← version history
├── guidelines/
│   ├── 01-brand-foundation.md     ← who we are, audience, pillars, voice & tone, vocabulary
│   ├── 02-visual-identity.md      ← logo, color palette (hex), typography
│   ├── 03-imagery.md              ← photography/illustration style, composition, do/don'ts
│   ├── 04-products.md             ← product catalog: names, NPK, claims, coverage, packaging
│   ├── 05-layout-and-channels.md  ← email + social anatomy, components, sizes, pre-flight check
│   └── 06-copywriting.md          ← headlines, CTAs, taglines, offer & subject-line formulas
├── prompts/
│   ├── image-prompt-library.md    ← ready-to-use AI image prompts by use case
│   └── style-tokens.md            ← reusable prompt fragments (palette, lighting, lens, negatives)
├── templates/
│   ├── email-templates.md         ← fill-in-the-blank email skeletons
│   └── social-templates.md        ← fill-in-the-blank social skeletons
├── assets/
│   ├── README.md                  ← naming + organization rules
│   ├── ASSET-LOG.md               ← registry of every asset (grows over time)
│   ├── logo/                      ← official logo files + links
│   ├── swatches/                  ← color swatch images
│   ├── references/                ← example layouts / screenshots
│   └── generated/                 ← NEW assets Claude Design creates go here
└── brand-board.html               ← open in a browser for a one-page visual summary
```

---

## Brand in 30 seconds

- **Who:** Yard Mastery — pro-grade lawn care products made for DIY homeowners. Built alongside **Allyn Hane, "The Lawn Care Nut" (LCN)** and a large DIY community.
- **Promise:** *"Build the Yard of Your Dreams"* — the same results the pros get, without the recurring service bill.
- **Pillars:** Pro Formulas · DIY Friendly · Real Results · Expert Support.
- **Voice:** Confident coach. Plain-spoken, encouraging, expert, a little fired-up. Talks to "you."
- **Look:** Bright, healthy turf green + harvest gold, bold uppercase headlines, clean product shots, real lawns and real results.
- **Core colors:** Green `#64B356` · Gold `#E0C030` · Action Green `#02AE65` · Sale Red `#D12442` · Ink `#191919`.
- **Type:** Roboto (headlines) + Lora (body).

> Full detail lives in the `guidelines/` files. This summary is just orientation.

---

## How to extend this system (keep it alive)

This is designed to grow. When you learn something new about the brand or create reusable work:

1. **New brand rule, color use, or pattern** → edit the relevant `guidelines/` file. Keep additions in the same format (rule + example + do/don't).
2. **New reusable image prompt that worked well** → add it to `prompts/image-prompt-library.md` under the right category, and note any new reusable fragment in `prompts/style-tokens.md`.
3. **New template** (a new email or social format you'll reuse) → add it to the relevant file in `templates/`.
4. **New asset you generated** (image, graphic, logo lockup) → save the file in `assets/generated/` using the naming rule in `assets/README.md`, then **add a row to `assets/ASSET-LOG.md`**.
5. **Anything you changed** → add a dated line to `CHANGELOG.md`.

**Formatting conventions for edits:** Markdown headings for scannability; hex codes in backticks; every guideline paired with a concrete *Do / Don't* where possible; product facts always cite the catalog. Write for a reader who will act on it — short, specific, example-driven.

---

## Source & maintenance

- **Built from:** the Yard Mastery email archive (Google Drive, 2025–2026 campaigns) + the live brand at [yardmastery.com](https://yardmastery.com).
- **Not yet connected:** the Yard Mastery Shopify store (auth required). Once connected, product data in `04-products.md` can be auto-synced (names, NPK, prices, pack contents, images). Until then, the catalog is sourced from the live site and is accurate as of the last update in `CHANGELOG.md`.
- **Owner:** Yard Mastery brand/design. Last updated: see `CHANGELOG.md`.
