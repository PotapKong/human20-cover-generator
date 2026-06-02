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
- bottom-left when the headline begins high or the hero dominates another zone;
- compact badge-only only when the composition is already text-heavy.

The logo block must align with the cover grid and surrounding spacing. It should not look like a late overlay.

## Mascot fidelity

For Human 2.0 covers and branded generated images, include the official mascot whenever the local asset exists at `references/images/maskot.jpg`, unless the user explicitly asks not to.

Treat the Human 2.0 mascot as an official brand asset, not a generic robot sticker.

The first generation must integrate the mascot into the scene itself. It should share the same lighting, shadow, perspective, reflections, and depth as the hero object or proof panel. Give it a useful role: operator, observer, tiny assistant, route-node companion, device-side helper, panel inspector, or foreground character interacting with the metaphor.

The mascot's small screen must keep the exact readable text:

`human20.app`

Do not blur, approximate, shorten, replace, or stylize this screen text. Avoid tiny mascot placement if the screen becomes unreadable.

If GPT Image cannot keep `human20.app` crisp at the chosen mascot size, use one of these fixes:

- scale the mascot up slightly;
- keep the mascot screen clean and perform a narrow correction pass for the exact `human20.app` text;
- correct only the screen text or a small distorted detail after generation.

Do not accept a cover where the mascot is visible but its screen is a glowing blob, random glyphs, or unreadable pseudo-text.

Do not paste the raw square `maskot.jpg` as a visible rectangular sticker. Do not solve a missing mascot by adding a detached circular avatar, badge, or PNG overlay. If the mascot is missing or sticker-like, regenerate with an explicit scene role.

Integrate the mascot as one of:

- a generated physical helper beside the hero object;
- a tiny operator touching a route node, device, switch, document, or product panel;
- a foreground scene character with natural contact shadow;
- a partially occluded assistant tucked behind a product panel or route node, still sharing the scene lighting.

The mascot should feel intentionally integrated with the cover grid and camera pass, not like a file dropped on top.

## Prompt wording

When an official asset is attached, write:

`Use the attached official Human 2.0 logo asset exactly as provided. Preserve the original aspect ratio. Place it in the bottom-left safe zone.`

When the official mascot is attached, requested, or available locally, add:

`Generate the Human 2.0 mascot as an organic part of the same scene, using the attached/local mascot as identity reference. Preserve its white glossy form, black face screen, blue glowing eyes, wing-like side fins, and tiny screen text human20.app. It must share the scene lighting, shadow, perspective, and reflections; do not paste it as a separate sticker, badge, avatar bubble, or overlay.`

## Checks

Before finalizing, check that:

- `H2.0` is spelled correctly.
- `Человек 2.0` is spelled correctly.
- `Среда внедрения ИИ` is spelled correctly.
- `human20.app` is readable on the mascot screen if the mascot is visible.
- the logo is not stretched or retyped.
- the mascot is not replaced with a generic robot.
- the mascot is physically integrated into the generated scene, not pasted on afterward.
- the logo does not compete with the main headline.
- the badge and text sit as one lockup, not as disconnected pasted elements.
