# 05 · Layout & Channels

How we assemble emails and social posts: the anatomy, reusable components, exact sizes per channel, and a pre-flight checklist. Pair with `templates/` for fill-in skeletons.

---

## 1. Email anatomy (the Yard Mastery promo pattern)

Our promo emails follow a repeatable top-to-bottom structure. Not every email uses every block — pick what the campaign needs.

1. **Pre-header / announcement strip** — tiny line: free shipping, sale name, or urgency.
2. **Hero** — one big image or color block + **bold UPPERCASE headline** (the promise or offer) + primary CTA button. The single most important block.
3. **Primary offer / product spotlight** — the featured product(s): product cutout(s), name with NPK, one-line benefit, price (with struck-through original if on sale), CTA.
4. **Supporting products grid** — 2–4 products, each = image + short name + its own CTA ("BUY HERE"). We repeat CTAs generously.
5. **Bundle / save callout** — "Save $$$ when you bundle," pack contents, savings %, CTA.
6. **"SALE INCLUDES" list** — when running a storewide sale: a scannable list of categories with % off (e.g., "Natural Nutrients 40% OFF · Bio-Stimulants 20% OFF · Packs 20% OFF"). High-converting, very on-brand.
7. **Education / App nudge** — "Check your calendar," soil-test tip, "Watch here" video link. Ties product to the App/expertise.
8. **Footer** — logo, company address (Bradenton, FL), social icons, **Unsubscribe**.

**Layout feel:** clean, single main column, generous white space, lots of green; product cutouts on white or light/green blocks; one clear primary CTA color (Action Green) with red reserved for sale/urgency.

### Reusable components (define once, reuse)
- **CTA button:** Action Green `#02AE65` fill, white **Roboto Bold UPPERCASE** label, rounded corners. Verbs: SHOP NOW / BUY HERE / SAVE HERE / LEARN MORE / WATCH HERE.
- **Price block:** big Roboto Black price; original price struck through; optional Sale Red "SAVE X%" or "$X OFF" flag.
- **Sale badge:** Sale Red `#D12442` chip, white bold text ("40% OFF," "ENDS TONIGHT").
- **Product card:** product image (transparent PNG ideal) + name w/ NPK + 1-line benefit + CTA.
- **Eyebrow/kicker:** small UPPERCASE letter-spaced label above a headline.
- **Coverage chip:** "18 lb · covers 6,000 sq ft."

---

## 2. Channel specs (sizes & aspect ratios)

> Verify platform specs before big launches — they drift. These are reliable defaults.

### Email
- **Body width:** 600px (max ~640px). Single column for mobile safety.
- **Hero image:** 1200×600px (2:1) exported @2x; keep text in the live HTML, not baked into the image, when possible.
- **Product cutouts:** transparent PNG, ~600px on the long edge.
- Always design **mobile-first** — most opens are on phones.

### Instagram
- **Feed square:** 1080×1080 (1:1)
- **Feed portrait:** 1080×1350 (4:5) — preferred for max feed real estate
- **Stories / Reels:** 1080×1920 (9:16) — keep text/CTA in the **middle 80%** (top/bottom get covered by UI)
- **Carousel:** 1080×1080 or 1080×1350 per slide

### Facebook
- **Feed image:** 1200×630 (1.91:1) or 1080×1080
- **Stories:** 1080×1920

### YouTube
- **Thumbnail:** 1280×720 (16:9) — big bold readable text, high contrast, expressive
- **Channel/hero art:** 2560×1440 (safe area 1546×423)

### X / Twitter
- **In-stream image:** 1600×900 (16:9)

### Pinterest (if used)
- **Pin:** 1000×1500 (2:3)

---

## 3. Layout do / don't
- **Do** keep one clear primary CTA per section; repeat the CTA down the email.
- **Do** use bold uppercase headlines and lots of green + white space.
- **Do** reserve **Sale Red** for sale/urgency only; use **Action Green** for normal CTAs.
- **Do** design mobile-first; big tap targets, legible at thumb size.
- **Don't** crowd multiple competing offers in one hero.
- **Don't** bake critical copy into a single flat image with no live text (hurts accessibility/deliverability) unless it's a social graphic.
- **Don't** use more than ~2 fonts or more than ~3 accent colors in one layout.

---

## 4. Pre-flight checklist (run before shipping anything)
- [ ] **Voice** matches `01-brand-foundation.md` (confident coach, "you," benefit-first)?
- [ ] **Colors/type** from `02-visual-identity.md` (Roboto headlines, brand green, Action-Green CTAs, red only for sale)?
- [ ] **Product names, NPK, claims, coverage** verified against `04-products.md`?
- [ ] **Prices / discount %** verified **live** (they change)?
- [ ] Correct **lawn-type framing** (warm vs cool) and **season**?
- [ ] **One clear primary CTA**; CTA verbs on-brand?
- [ ] Correct **aspect ratio/size** for the channel?
- [ ] Image passes the **imagery checklist** (`03-imagery.md`) — real greens, space for logo, no garbled text/logos?
- [ ] Logo used per rules; real logo composited (not AI-rendered)?
- [ ] (Email) address + **Unsubscribe** present?
- [ ] New asset **saved to `assets/generated/` and logged** in `ASSET-LOG.md`?
