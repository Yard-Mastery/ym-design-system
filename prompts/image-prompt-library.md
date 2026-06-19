# Image Prompt Library

Ready-to-use AI image prompts for Yard Mastery, organized by use case. **How to use:** pick a recipe, swap the `[BRACKETS]`, then append the shared fragments from `style-tokens.md` (BASE_STYLE + LIGHTING + ASPECT + NEGATIVE). Every recipe already assumes the Yard Mastery look from `03-imagery.md`.

> **Always:** generate with clean space for headline + logo; never let the model render the logo or important text — composite real assets after. See the TEXT-IN-IMAGE policy in `style-tokens.md`.

**Legend:** `[PRODUCT]` = full product name w/ NPK from `04-products.md` · `[SEASON]` · `[GRASS]` = warm/cool-season · `[AR]` = aspect ratio for the channel.

---

## 1. Product hero — e-commerce (white background)
For clean catalog/product-spotlight cutouts.
```
Professional studio product photograph of a [PRODUCT] bag/bottle, centered on a seamless pure-white
background, soft studio softbox lighting with gentle reflection beneath, slight low heroic angle,
ultra-sharp, true-to-life packaging colors (Yard Mastery green & gold bag).
Studio softbox lighting on seamless white. shot on 90mm, crisp focus. centered with even margin.
[AR=1:1]. + BASE_STYLE + NEGATIVE_PROMPT
```
Variations: "both bag sizes side by side (18 lb and 45 lb)"; "with a small pile of fertilizer granules in front"; "3/4 angle showing front and side."

## 2. Product on the lawn (in context, hero)
The signature Yard Mastery shot.
```
A [PRODUCT] bag standing upright on a freshly mowed, lush striped green [GRASS] lawn, a tidy
suburban American home softly blurred in the background, warm inviting atmosphere.
golden hour, warm low sun, soft long shadows. shot on 50mm, shallow depth of field, bag sharp,
background blurred. leave clean empty space in the top third for headline. [AR=4:5].
+ BASE_STYLE + COLOR_DIRECTION + NEGATIVE_PROMPT
```

## 3. Product in use / action (how-to energy)
```
Close-up of a homeowner's hands [ACTION: pushing a broadcast spreader spreading granular fertilizer
across a green lawn / spraying liquid lawn treatment with a backpack sprayer / holding a soil test
kit and a plug of soil], dynamic and authentic, motion of granules/spray visible, healthy green
turf, suburban backyard.
bright open daylight. 35mm, deep focus. action to one side, open space opposite for copy. [AR=16:9].
+ BASE_STYLE + PEOPLE direction + NEGATIVE_PROMPT
```
Action swaps: spreading granules · spraying (backpack/hose-end) · mowing stripes · raking/seeding · watering.

## 4. Lifestyle / lawn pride ("memories are made")
```
A happy American family [or: a man with his dog / kids playing / friends at a backyard BBQ] enjoying
a beautiful thick green backyard lawn on a warm afternoon, relaxed candid moment, suburban home,
sense of pride and comfort.
golden hour, warm glow. 35mm environmental, natural depth. composition leaves sky/space at top for
headline. [AR=4:5]. + BASE_STYLE + PEOPLE direction + NEGATIVE_PROMPT
```

## 5. Results / proof (turf close-ups & before/after)
```
Extreme macro close-up of healthy [GRASS] grass blades, deep rich green, morning dew droplets,
perfect density and color, shallow focus falling off softly.
90mm macro, soft morning light. fills frame with clean top space. [AR=16:9].
+ BASE_STYLE + COLOR_DIRECTION + NEGATIVE_PROMPT
```
Before/after: generate as **two separate images** (a thin/patchy pale lawn, then a thick dark-green lawn from the same angle) and composite a split with a divider in layout — don't ask the model for a single split image (results look fake).

## 6. Color / "Double Dark" showcase
```
A striking dark blue-green [GRASS] lawn with crisp mowing stripes leading to a suburban home,
showing off deep premium color (Double Dark look), rich and saturated but natural.
late golden hour. wide 35mm, low angle along the stripes. headline space in upper third. [AR=16:9].
+ BASE_STYLE + NEGATIVE_PROMPT
```

## 7. Seasonal themes

**Spring (pre-emergent / green-up):**
```
Early-spring suburban lawn just greening up, fresh and cool, dew on grass, budding trees, a broadcast
spreader on the lawn ready for pre-emergent application. fresh morning light. 35mm. open sky for text. [AR=4:5].
+ BASE_STYLE + NEGATIVE_PROMPT
```
**Summer (heat & drought):**
```
A vibrant green lawn thriving in high summer heat, sprinkler mist catching warm sunlight, deep blue
sky, resilient turf, sense of "beating the heat." bright warm sun. 50mm, shallow DOF. text space left. [AR=16:9].
+ BASE_STYLE + NEGATIVE_PROMPT
```
**Fall (seeding / overseed):**
```
Autumn cool-season lawn at golden hour, a few fallen leaves at the edges, homeowner overseeding with a
spreader, warm low light, cozy seasonal mood. golden hour. 35mm. clean top space for headline. [AR=4:5].
+ BASE_STYLE + NEGATIVE_PROMPT
```
**Winter / Holiday (Christmas lights line):**
```
A tidy suburban home at dusk with tasteful warm-white C9 Christmas lights along the roofline, crisp
winter evening, inviting glow, dormant lawn in foreground. blue-hour + warm bulb glow. 35mm. [AR=16:9].
+ BASE_STYLE + NEGATIVE_PROMPT
```

## 8. Social graphic backgrounds (for promos/sales)
Generate a clean branded **background** to drop text/product/CTA onto in layout.
```
Minimal branded background graphic: smooth gradient from Yard Mastery green (#64B356) to deep turf
green (#1E5631), subtle abstract grass-blade or organic texture in a lower corner, lots of clean
empty space for headline and product cutout, modern and premium, flat commercial design (no text).
[AR per channel]. + NEGATIVE_PROMPT (especially: no text, no logos)
```
Variations: "white background with a green diagonal color block and a soft shadow for a product cutout"; "harvest-gold accent banner shapes"; "Sale Red ribbon shape for a discount badge" (badge art only, add the number in layout).

## 9. YouTube thumbnail base
```
High-impact YouTube thumbnail background: a dramatic, super-green striped lawn with a bright sky,
strong depth and contrast, an expressive homeowner reacting with excitement on one side, big clean
empty area on the opposite side for large bold text added later. punchy bright lighting, high contrast,
saturated but natural. 16:9. + BASE_STYLE + PEOPLE direction + NEGATIVE_PROMPT
```

## 10. App promotion
```
A smartphone held in a hand outdoors on a green lawn, screen area left blank/clean (to composite the
Yard Mastery App UI later), bright suburban backyard softly blurred behind, modern and friendly.
bright daylight. 50mm shallow DOF. phone to one side, copy space opposite. [AR=1:1].
+ BASE_STYLE + NEGATIVE_PROMPT  (leave the phone screen empty for app screenshot compositing)
```

## 11. Organics / garden line
```
A home vegetable and flower garden flourishing — ripe tomatoes, leafy greens, colorful blooms, rich
dark soil — with space for a product, natural and wholesome, "grow better food & flowers" feeling.
warm natural light. 35mm. clean corner space. [AR=4:5]. + BASE_STYLE + NEGATIVE_PROMPT
```

---

## Quick-fill recipes for hero products
Paste, then add LIGHTING + AR + NEGATIVE from `style-tokens.md`.

- **Flagship 24-0-6** (everyday green): *"Flagship 24-0-6 bag on a thick, striped, all-purpose green lawn, suburban home behind, golden hour, room for headline up top."*
- **Stress Blend 7-0-20** (summer): *"Stress Blend 7-0-20 bag on a resilient green lawn under bright summer sun, sprinkler mist, heat-survival mood, text space left."*
- **Double Dark 16-0-0** (color): *"Double Dark 16-0-0 bag on a deep blue-green striped lawn at dusk golden hour, premium dark color showcase."*
- **Prodiamine 0-0-7** (spring weed prevention): *"Prodiamine pre-emergent bag with a broadcast spreader on an early-spring lawn, crabgrass-prevention theme, fresh morning light."*
- **Soil Test Kit:** *"Yard Mastery soil test kit box with a soil probe and a plug of soil on a green lawn, clean how-to styling, bright open shade."*
- **Backpack Sprayer** (Father's Day): *"Homeowner spraying the lawn with the 4-gallon backpack sprayer, action shot, warm afternoon, 'spray like the pros' energy, copy space opposite."*

> After generating: run the **imagery checklist** (`03-imagery.md`), composite real logo/text, save to `assets/generated/`, and log it in `assets/ASSET-LOG.md`.
