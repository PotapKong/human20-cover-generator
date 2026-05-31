# Human 2.0 Visual System

Use this reference to keep generated images close to the current Human 2.0 cover language.

## Signature cover layout

Use this layout for Dzen / Telegram / article covers:

- Light gray canvas `#F3F4F6`.
- Large bold headline on the left, usually 2-3 lines.
- One accent word or phrase in indigo `#6366F1`.
- Main visual object or white rounded panel on the right.
- Thin indigo connector lines, small circular nodes.
- Small official H2.0 / Human 2.0 logo asset in the bottom-left safe zone.
- Optional 3x3 dot pattern in top-right or bottom-left.
- Tiny gold `#C4A148` accent only as dot, spark, checkmark, or divider.
- Generous negative space.
- Soft shadow under white surfaces.
- Editorial/product-slide feel, not generic SaaS illustration.

## Official color system

Use the official Human 2.0 brandbook as the source of truth: `human20.app/brand`.

Palette:

- Accent / H2.0 sign: `#6366F1`
- Primary text: `#2C2C2C`
- Canvas background: `#F3F4F6`
- Surface background: `#FFFFFF`
- Gold accent: `#C4A148`

The primary accent is always indigo/blue `#6366F1`. Use it for highlighted words, connector lines, nodes, arrows, progress bars, active UI states, and badges.

Gold `#C4A148` is secondary and should stay tiny: one dot, small spark, small checkmark, minor divider, or micro-highlight.

Do not use green as a Human 2.0 accent color. Green is allowed only if it is part of a real screenshot or official third-party UI that must be preserved. When adapting UI cards into the Human 2.0 style, replace non-essential green accents with indigo/blue.

## Visual hierarchy

1. Headline first.
2. One metaphor second.
3. Brand mark third.
4. Decorative UI details last.

Do not make the viewer decode a complex schema before understanding the claim.

## Typography

- Headline: ultra-condensed poster/display grotesk when references show it; very tall narrow glyphs, tight line-height, hard vertical strokes, uppercase or near-uppercase.
- Do not use Geologica for the main headline when the reference examples use the ultra-condensed style; Geologica is too wide/soft and should be reserved for secondary brand/support text or non-reference fallback work.
- Durable headline font order: exact user/repo-bundled licensed display font first, `assets/brand/h20-display-condensed.ttf` if present, then an available licensed ultra-condensed Cyrillic display face with comparable proportions.
- If exact typography matters, generate the scene without headline text and composite the headline manually from the chosen font. Reject results where the headline looks wide, rounded, soft, or Geologica-like.
- Body/captions: Onest-like.
- Avoid long subtitles inside image.
- If text is generated inside image, use no more than 5-7 words.
- Prefer manual typography or clean empty space for complex headlines.

## Brand footer

Use one of:

- official PNG/SVG `H2.0` badge + `Человек 2.0 / Среда внедрения ИИ`
- official compact `H2.0` badge only if space is tight
- plain text fallback `Человек 2.0 · Среда внедрения ИИ` if no official logo asset is available

Never ask the image model to redraw the official logo from memory. If the exact PNG/SVG asset is not available, leave space for manual logo placement or use the plain text fallback.

Never write:

- `Human20` as public brand replacement
- `H 2.0`
- `H-2.0`
- `AI` in Russian copy, except official names, URLs, citations, or fixed product names

## Reference-like details

Good Human 2.0 covers often include:

- oversized black headline with one indigo keyword
- white rounded cards, panels, or dashboard surfaces
- one continuous indigo route line from input to output
- small gold validation dot or spark
- reduced UI text represented as abstract bars
- premium restraint: no unnecessary labels, no busy backgrounds

## Hyperreal integration

When adding a hyperreal object, keep it as the single hero object:

- crown, glass robot, iceberg, notebook, physical card, device, control dial, or cinematic UI object
- shallow depth of field and soft blur are allowed
- object lighting may use subtle indigo/gold reflections
- do not turn the image into cyberpunk, neon, sci-fi poster, or stock-photo collage
