# 02 · Visual Identity

Logo, color, and type. These are the non-negotiable building blocks of every visual. **Load this for every piece of content.**

> Colors and fonts below were sampled directly from the live logo and yardmastery.com. "Observed" = pulled from the brand; "Extended" = recommended additions for depth in imagery/graphics (use freely, but the Observed core is what makes it unmistakably Yard Mastery).

---

## 1. Color palette

### Core brand (Observed)
| Name | Hex | RGB | Use |
|---|---|---|---|
| **Yard Mastery Green** | `#64B356` | 100, 179, 86 | Primary brand color. Links, accents, headlines on dark, brand fields. (Logo green ≈ `#60B050`.) |
| **Harvest Gold** | `#E0C030` | 224, 192, 48 | Secondary brand color (from the logo mark). Accents, highlights, "sun/grow" energy, badges. |

### Action & state (Observed)
| Name | Hex | RGB | Use |
|---|---|---|---|
| **Action Green** | `#02AE65` | 2, 174, 101 | Primary CTA buttons ("BUY," "SHOP," "SAVE"). Brighter/cleaner than brand green for max click contrast. |
| **Sale Red** | `#D12442` | 209, 36, 66 | Sale prices, % off, urgency, clearance badges, "ends tonight." Use sparingly for punch. |
| **Energy Orange** | `#FF8B21` | 255, 139, 33 | Secondary highlights, seasonal warmth, attention flags. Pairs with green for fall/heat themes. |

### Neutrals (Observed)
| Name | Hex | Use |
|---|---|---|
| **Ink** | `#191919` | Near-black for text, dark blocks/footers, high-contrast headlines. |
| **True Black** | `#000000` | Body text on white. |
| **Slate** | `#3C3C3C` | Secondary text, captions. |
| **White** | `#FFFFFF` | Primary background, reverse text on green/ink. |
| **Mist Gray** | `#F4F5F2` | *(Extended)* Soft section backgrounds, cards. |
| **Line Gray** | `#E3E5E0` | *(Extended)* Dividers, borders. |

### Extended greens & scene colors (Extended — for imagery, gradients, depth)
| Name | Hex | Use |
|---|---|---|
| **Deep Turf Green** | `#1E5631` | Dark green for backgrounds, depth, gradients, text on light. Anchors the palette. |
| **Fresh Sod** | `#8CD06B` | Light, lush highlight green (new growth, gradients). |
| **Sky** | `#7FB8E6` | Outdoor scene skies (use only as a scene element, not a brand color). |
| **Soil Brown** | `#5A3E2B` | Earth/soil context in product/scene imagery. |

### Palette usage rules
- **60 / 30 / 10:** ~60% neutral (white/mist), ~30% brand green family, ~10% accent (gold/orange/red) per composition. Don't let red/orange dominate.
- **Green = brand & "go." Red = sale & urgency only.** Never use Sale Red as a general decorative color.
- **Contrast/accessibility:** body text should hit **WCAG AA (4.5:1)**. `#64B356` is a mid-tone — do **not** put small white or black text on it for body copy; use Ink/Deep Turf Green text, or reserve brand green for large headlines/blocks. For buttons, white text on **Action Green `#02AE65`** passes for large/bold button labels; verify small text.
- **Dark mode / dark blocks:** Ink `#191919` or Deep Turf Green `#1E5631` background, white headlines, Harvest Gold or Fresh Sod accents.
- Swatch reference image: `assets/swatches/ym-color-palette.png`. Interactive: open `brand-board.html`.

---

## 2. Typography

**Two-typeface system** (both are free Google Fonts — safe for web, email, and image generation):

| Role | Typeface | Weights | Notes |
|---|---|---|---|
| **Headlines / display / UI** | **Roboto** | Black (900), Bold (700), Medium (500) | Our workhorse. Promotional headlines are typically **BOLD, UPPERCASE, tight tracking** for impact. Roboto Condensed is great for dense promo lockups. |
| **Body / editorial** | **Lora** | Regular (400), Medium (500), Bold (700) | Serif. Used for body copy, longer-form/editorial, and a warmer, premium feel. |
| **Fallback / utility** | Arial / Helvetica | — | System fallback for buttons and where Roboto isn't available. |

### Email- & web-safe font stacks
```css
/* Headlines */
font-family: "Roboto", Arial, Helvetica, sans-serif;
/* Body */
font-family: "Lora", Georgia, "Times New Roman", serif;
```

### Type hierarchy (starting scale — adjust per layout)
| Level | Font / weight | Email size | Social/graphic feel |
|---|---|---|---|
| Hero headline | Roboto Black, UPPERCASE | 32–44px | Big, dominant, often over image |
| Subhead | Roboto Bold | 22–28px | Supporting promise/benefit |
| Section label / eyebrow | Roboto Bold, UPPERCASE, letter-spaced | 12–14px | Small kicker above headline |
| Body | Lora Regular | 15–17px / 1.5 | Readable, friendly |
| CTA button label | Roboto Bold, UPPERCASE | 14–16px | e.g., "SHOP NOW" |
| Price / offer | Roboto Black | 24–40px | Big number; strike old price |
| Legal / footer | Roboto or Lora Regular | 11–12px | Slate/gray |

### Type do / don't
- **Do** set promo headlines in bold uppercase Roboto; keep them short (3–7 words).
- **Do** pair a Roboto headline with Lora body for contrast.
- **Don't** introduce off-brand display fonts (no script, no novelty fonts) unless a campaign explicitly calls for it.
- **Don't** set long body copy in all caps.

---

## 3. Logo

**Official logo (color):** the "YM" mark + "YARD MASTERY" wordmark in green & gold.

Canonical files (Shopify CDN — public, always current). Use these directly or download into `assets/logo/`:
- 480px: `https://yardmastery.com/cdn/shop/files/YM_Logo_Color_d568a775-f4b0-4345-8dce-49f2c2142979_480x.png`
- 115px: `https://yardmastery.com/cdn/shop/files/YM_Logo_Color_d568a775-f4b0-4345-8dce-49f2c2142979_115x.png`
- 50px: `https://yardmastery.com/cdn/shop/files/YM_Logo_Color_d568a775-f4b0-4345-8dce-49f2c2142979_50x.png`

(See `assets/logo/README.md` for the current local copy and any added variations like white/knockout.)

### Logo usage rules
- **Clear space:** keep padding of at least the height of the "Y" on all sides. Never crowd it.
- **Minimum size:** ~120px wide on screen / ~1 inch in print so the wordmark stays legible.
- **Backgrounds:** prefer the color logo on **white or light** backgrounds. On dark/photo backgrounds, use a **white/knockout** version (add to `assets/logo/` when created) or place the color logo on a solid light chip.
- **Don't:** stretch/squash, rotate, recolor, add shadows/outlines, place on busy photo areas with low contrast, or recreate the wordmark in a different font.
- **In AI-generated images:** do **not** ask the image model to render the logo or text — models garble logos/letterforms. Generate the image with clean negative space (top or a corner), then **composite the real logo file** on top in layout. (See `prompts/image-prompt-library.md`.)

### Co-brand
**The Lawn Care Nut (LCN)** mark appears in community content and on select products. Keep YM as the primary brand; LCN is secondary/endorsing. Don't merge the two logos into one lockup.

---

## 4. Quick reference (copy-paste tokens)
```
Green        #64B356   (logo green #60B050)
Gold         #E0C030
Action Green #02AE65
Sale Red     #D12442
Energy Orange#FF8B21
Ink          #191919
Slate        #3C3C3C
White        #FFFFFF
Deep Turf    #1E5631   (extended)
Fresh Sod    #8CD06B   (extended)
Headlines: Roboto (Black/Bold, UPPERCASE for promo)
Body: Lora (serif)
```
