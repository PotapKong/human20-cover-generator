# Accent Color Discipline

Use the official Human 2.0 brandbook as the source of truth for colors: `human20.app/brand`.

## Official palette

- Flat accent / H2.0 blue: `#2C44F5`
- H2.0 mark gradient: `#6C84FF -> #2C44F5`
- Primary text: `#2C2C2C`
- Canvas background: `#F3F4F6`
- Surface background: `#FFFFFF`
- Gold accent: `#C4A148`

## Priority

For Human 2.0 covers and infographics, use colors in this order:

1. Light gray canvas `#F3F4F6`
2. White cards and panels `#FFFFFF`
3. Graphite typography `#2C2C2C`
4. Brand blue accent `#2C44F5`
5. Tiny gold accent `#C4A148`

## Main rule

The primary flat accent is always brand blue `#2C44F5`. Use it for:

- highlighted headline words
- connector lines
- nodes and dots
- active UI states
- progress bars
- check marks
- small badges
- arrows
- card accents

`#6C84FF` is allowed only as the light side of the official H2.0 logo/mark gradient or as a subtle blue glow that still resolves toward `#2C44F5`. It is not the main headline color.

## Gold usage

Gold `#C4A148` is secondary. Use it only for tiny details:

- one dot in a 3x3 pattern
- tiny spark
- small check mark
- small divider
- minor highlight

Do not use gold as the main interface color, main headline color, or large background fill.

## Green usage

Do not use green as a Human 2.0 accent color.

Green is allowed only when:

- it is part of a real screenshot or official third-party UI that must be preserved
- it is a tiny status indicator inside a preserved screenshot
- the user explicitly asks for green

When adapting screenshots or UI cards into the Human 2.0 style, replace non-essential green accents with brand blue `#2C44F5`.

## Avoid

- neon green as a main accent
- lime interface styling
- cyberpunk green/black palette
- generic SaaS purple gradients
- purple, violet, lavender, or generic indigo accents
- Tailwind-style `#6366F1`, which drifts too purple for Human 2.0
- full gold UI
- random extra colors outside the brand palette

## Prompt wording

Use this wording in generation prompts when color drift is a risk:

`Use the official Human 2.0 palette only: light gray #F3F4F6, white #FFFFFF, graphite #2C2C2C, brand blue #2C44F5 as the only primary flat accent, optional official mark gradient #6C84FF -> #2C44F5 only for logo/glow, and tiny gold #C4A148 accents. Do not use purple, violet, generic indigo, #6366F1, or green as an accent except green inside preserved real screenshots.`

## Quality check

Before finalizing:

- Are all custom UI accents brand blue `#2C44F5`, not purple/violet/generic indigo/green?
- Is `#6366F1` absent from headline accents, routes, nodes, and UI highlights?
- Is gold used only as a tiny accent?
- Does the cover still read as Human 2.0 rather than cyberpunk, SaaS purple, or green tech branding?
- If a screenshot contains green, is it clearly part of the screenshot rather than the Human 2.0 layout?
