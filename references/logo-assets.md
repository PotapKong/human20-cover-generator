# Logo Asset Rules

Use the official brandbook page `human20.app/brand` as the source of truth for Human 2.0 logo assets.

Local official assets may be bundled in `assets/brand/`:

- `h20-lockup-dark.svg`
- `h20-lockup-light.svg`
- `h20-stack-dark.svg`
- `h20-mark.svg`
- `h20-lockup-dark-1440.png`
- `h20-mark-512.png`

## Main rule

For covers and infographics, use the official PNG or SVG logo asset whenever the logo must be visible. Preserve the original aspect ratio and spacing.

The image model should not recreate the logo from memory. If exact logo fidelity matters, generate with clean space and composite the official PNG/SVG after generation. If no logo asset is attached or available, leave clean space for manual logo placement or use a plain text footer: `Человек 2.0 · Среда внедрения ИИ`.

## Placement

- 16:9 cover: bottom-left safe zone.
- 9:16 Reels cover: bottom safe zone.
- Infographic: small footer, only if readable.

For horizontal covers, prefer an integrated lockup:

- H2.0 badge on the left, `Человек 2.0` and `Среда внедрения ИИ` to the right;
- top-left when the hero object dominates the right side;
- bottom-left when the headline begins high on the left;
- compact badge-only only when the composition is already text-heavy.

The logo block must align with the cover grid and surrounding spacing. It should not look like a late overlay.

## Prompt wording

When an official asset is attached, write:

`Use the attached official Human 2.0 logo asset exactly as provided. Preserve the original aspect ratio. Place it in the bottom-left safe zone.`

## Checks

Before finalizing, check that:

- `H2.0` is spelled correctly.
- `Человек 2.0` is spelled correctly.
- `Среда внедрения ИИ` is spelled correctly.
- the logo is not stretched or retyped.
- the logo does not compete with the main headline.
- the badge and text sit as one lockup, not as disconnected pasted elements.
