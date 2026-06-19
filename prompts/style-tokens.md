# Style Tokens — reusable prompt fragments

Copy-paste building blocks for AI image generation. Combine a **subject** (from `image-prompt-library.md`) with the **base style**, the right **lighting/lens**, an **aspect ratio**, and the **negative prompt**. Keeping these consistent is what makes every image look like Yard Mastery.

> Works with any modern image model (e.g., the imagegen skill, Midjourney, DALL·E, Firefly, Ideogram). For models without a `--ar` flag, state the aspect ratio in words ("vertical 4:5 composition").

---

## BASE_STYLE (append to almost every prompt)
```
Yard Mastery brand style: bright, healthy, photorealistic American lawn-care imagery.
Lush, vibrant-but-natural green turf, warm natural daylight, clean and aspirational yet
believable. Crisp focus on the subject, uncluttered composition, generous negative space
for headline and logo. High-end commercial product/lifestyle photography. Realistic textures.
```

## COLOR_DIRECTION
```
Color palette anchored in Yard Mastery green (#64B356) and harvest gold (#E0C030); healthy
saturated greens, warm whites, natural earth tones. Avoid neon/alien greens.
```

## LIGHTING options
- `golden hour, warm low sun, soft long shadows, optimistic glow` ← default hero
- `bright open shade, soft even daylight, true-to-life color` ← clean product/how-to
- `clear midday sun on green turf, vivid and fresh` ← results/proof
- `studio softbox lighting on seamless white, soft reflections` ← e-comm product cutout

## LENS / CAMERA options
- `shot on 50mm, shallow depth of field, subject sharp, background softly blurred` ← hero product/action
- `35mm environmental shot, deep focus` ← lifestyle/scene
- `90mm macro, extreme close-up, dew detail` ← turf/granule texture
- `slight low angle, heroic` ← product hero / bag
- `top-down flat lay` ← kit/tools arrangement

## COMPOSITION / NEGATIVE SPACE
- `leave clean empty space in the top third for headline text` (hero)
- `subject positioned to the right, open space on the left for copy`
- `centered subject with even margin for a 1:1 social post`
- `keep key elements within the middle 80% (safe area) for a 9:16 story`

## ASPECT RATIOS (by channel — see 05-layout-and-channels.md)
- Email hero / YouTube / X: `16:9` (or 2:1 for email hero banners)
- Instagram feed: `4:5` (preferred) or `1:1`
- Stories / Reels: `9:16`
- Pinterest: `2:3`

## NEGATIVE_PROMPT (always include)
```
no text, no words, no lettering, no logos, no watermarks, no brand names, no garbled type;
no fake neon/radioactive green, no plastic-looking grass, no dead/patchy/weedy lawn (unless requested);
no competitor products or big-box bags; no cluttered background; no dim/gloomy/cold-blue lighting;
no stiff stock-photo poses; no distorted hands or faces; not cartoonish, not over-saturated, not HDR-halos.
```

## PEOPLE direction (when including a person)
```
everyday American homeowner, casual weekend clothes, ages 30-65, diverse, genuine candid expression
of pride/focus, hands-on with the lawn; natural body proportions; authentic, not posed.
```

## SEASON modifiers (drop in as needed)
- **Spring:** `early spring, fresh green-up, tulips/budding trees, cool morning light`
- **Summer:** `high summer, deep green lawn, bright warm sun, sprinkler mist, heat-and-drought theme`
- **Fall:** `autumn, golden hour, a few fallen leaves, overseeding/seeding theme, cool-season grass`
- **Winter/Holiday:** `crisp winter light, tasteful Christmas lights on a suburban home at dusk, cozy`

## TEXT-IN-IMAGE policy
Do **not** ask the model to render headlines, prices, or the logo (models garble them). Generate the photographic/graphic base with reserved negative space, then **composite real text + the real logo** in layout. If a model *must* include a short word (e.g., Ideogram for typographic posters), keep it to 1–3 words, verify spelling, and still composite the official logo separately.

## HOW TO ASSEMBLE A PROMPT
```
[SUBJECT from image-prompt-library] , [SEASON modifier if any] ,
BASE_STYLE , COLOR_DIRECTION , [LIGHTING] , [LENS] , [COMPOSITION/negative space] ,
[ASPECT RATIO]  ||  Negative: NEGATIVE_PROMPT
```
Example:
```
A 45 lb Yard Mastery Flagship 24-0-6 fertilizer bag standing on a freshly mowed striped
green lawn, suburban home softly blurred behind. golden hour, warm low sun, soft long shadows.
shot on 50mm, shallow depth of field. leave clean empty space in the top third for headline.
4:5.  Bright healthy photorealistic Yard Mastery style, greens natural not neon, harvest-gold
accents, aspirational yet believable.
Negative: no text, no logos, no garbled type, no neon grass, no clutter, no competitor brands.
```
