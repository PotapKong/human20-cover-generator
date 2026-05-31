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

## Mascot fidelity

If the Human 2.0 mascot is used, treat it as an official brand asset, not a generic robot sticker.

The mascot's small screen must keep the exact readable text:

`human20.app`

Do not blur, approximate, shorten, replace, or stylize this screen text. Avoid tiny mascot placement if the screen becomes unreadable.

If GPT Image cannot keep `human20.app` crisp at the chosen mascot size, use one of these fixes:

- scale the mascot up slightly;
- keep the mascot screen clean and perform a narrow correction pass for the exact `human20.app` text;
- composite the official mascot or corrected screen text after generation.

Do not accept a cover where the mascot is visible but its screen is a glowing blob, random glyphs, or unreadable pseudo-text.

## Prompt wording

When an official asset is attached, write:

`Use the attached official Human 2.0 logo asset exactly as provided. Preserve the original aspect ratio. Place it in the bottom-left safe zone.`

When the official mascot is attached or requested, add:

`Use the attached official Human 2.0 mascot exactly as provided. Preserve its identity and proportions. The small screen on the mascot must read exactly: human20.app. Keep this text crisp and readable; if the mascot is too small, enlarge it or leave the screen for a correction pass.`

## Checks

Before finalizing, check that:

- `H2.0` is spelled correctly.
- `Человек 2.0` is spelled correctly.
- `Среда внедрения ИИ` is spelled correctly.
- `human20.app` is readable on the mascot screen if the mascot is visible.
- the logo is not stretched or retyped.
- the mascot is not replaced with a generic robot.
- the logo does not compete with the main headline.
- the badge and text sit as one lockup, not as disconnected pasted elements.
