# Anti-patterns

Use this file when refining a generation or before generating an image where exact brand and text fidelity matters.

## Logo fidelity

Do not invent or redraw the Human 2.0 logo. If the logo must be visible, use the official PNG/SVG asset from `human20.app/brand` and preserve its original aspect ratio.

If the official asset is not attached or available, use a safe fallback:

- leave clean space for manual logo placement
- use plain text: `Человек 2.0 · Среда внедрения ИИ`
- use a simple `H2.0` text badge only if the user accepts approximation

Correct text:

- `H2.0`
- `Человек 2.0`
- `Среда внедрения ИИ`

Avoid:

- `Human20` as a public brand replacement
- `H 2.0`
- `H-2.0`
- changed badge proportions
- generated logo redraws
- stretched footer badges
- corrupted brand text

## Color drift

Do not drift away from the Human 2.0 brand palette.

Correct palette:

- indigo/blue `#6366F1` as the primary accent
- graphite `#2C2C2C` for text and dark lines
- light gray `#F3F4F6` for canvas
- white `#FFFFFF` for surfaces
- tiny gold `#C4A148` only as a secondary micro-accent

Avoid:

- green or lime as primary accent
- cyberpunk green/black styling
- generic purple gradients
- large gold fills
- random extra colors

Green is allowed only inside a preserved real screenshot or official third-party UI. If the UI card is being adapted to Human 2.0, replace green status indicators, progress bars, and code highlights with indigo/blue.

## Russian copy

In Russian copy, write `ИИ`, not `AI`, except official English names, URLs, citations, direct quotes, or unchanged product names.

Use:

- `ИИ-агенты`
- `ИИ-образование`
- `ИИ-инструменты`

## Text volume

Do not generate long subtitles, source lines, tables, or tiny UI labels inside images.

Use:

- one headline
- optional 1 short caption
- abstract bars instead of fake UI paragraphs

## Generic SaaS look

Avoid generic purple dashboards, random floating cards with meaningless labels, generic robot brain visuals, stock tech blobs, and blue/purple neon sci-fi styling.

Replace with:

- Human 2.0 white surfaces
- indigo route lines
- small gold accents
- one grounded metaphor from the article

## Thumbnail strength

For Dzen and Instagram, the headline must be readable at small size.

Avoid thin fonts, small captions as the main idea, too many lines, and low contrast text.

## Overexplained infographic

Do not visualize every article point. Choose one editorial claim.

Bad direction: 8 cards, 12 arrows, 4 logos, 20 labels.
Good direction: one input, one transformation, one outcome.

## Russian text reliability

If Russian text must be exact, keep it short. If the phrase is complex, generate the image with clean space and add text manually later.

Safe text lengths:

- 1-4 words: usually safe
- 5-7 words: acceptable
- 8+ words: higher risk

## Crop and safe zones

For Reels, keep the main phrase in the top/middle safe area and do not place important brand or text at extreme edges.

For outpainting, preserve the existing graphic and extend only the background.

## Gold usage

Gold is a secondary accent, not the main UI color. Use it for small dots, sparkles, dividers, or one hero object when the metaphor requires it, such as a crown.