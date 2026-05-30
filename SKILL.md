---
name: human20-cover-generator
description: Create premium Human 2.0 branded article, Telegram, Dzen, Instagram/Reels, and social cover images from a post/article text. Use when the user asks to придумать/сгенерировать/перегенерировать баннер, обложку, картинку, cover, image, illustration, инфографику, vertical reels cover, or заменить перегруженную инфографику for a text; when they want a short Russian headline on the image; when they mention Human 2.0 brand style, brandbook, logos, mascots, GPT Image, or fitting a provided image/logo into a clean Human 2.0 layout.
---

# Human 2.0 Cover Generator

## Overview

Turn article/post text into a premium, minimal, editorial Human 2.0 visual. Prefer one clear idea, one short headline, one strong metaphor, and a restrained brand-system composition over dense infographics.

If the user asks to generate immediately, use the built-in image generation flow after shaping the concept. Do not stop at a prompt unless the user asks only for a prompt.

## Core Workflow

1. Read the supplied text and extract the central editorial claim, not every detail.
2. Choose the audience mode:
   - `Mass audience` for Dzen, Instagram, Telegram, entrepreneurs, creators, and non-technical readers.
   - `Editorial / expert` for readers who already follow ИИ tools and product names.
   - `Technical` only when the post is clearly for developers or the user asks for a technical cover.
3. Choose the generation mode:
   - `Dzen / Telegram cover` for 16:9 article thumbnails.
   - `Instagram / Reels cover` for 9:16 vertical covers.
   - `Clean infographic` for tables, charts, comparison cards, or data visuals.
   - `Premium object cover` when the user asks for a more Instagram-native, cinematic, or hyperreal image.
   - `Refinement` when fixing a failed generation, typography, crop, logo, or brand mismatch.
4. Read the relevant references before prompting:
   - `references/headline-patterns.md` before choosing the headline.
   - `references/logo-assets.md` before adding any Human 2.0 logo or footer.
   - `references/reference-gallery.md` first, to choose the closest proven Human 2.0 archetype.
   - `references/visual-system.md` for the Human 2.0 visual language.
   - `references/formats.md` for aspect ratio and safe-zone rules.
   - `references/generation-modes.md` for image prompt mode.
   - `references/anti-patterns.md` when refining or avoiding recurring failures.
   - `references/cover-patterns.md` when choosing between several concepts or improving a weak metaphor.
5. Choose one short Russian headline that is understandable in a feed. For broad-audience covers, lead with benefit or use case, not tool internals.
6. Choose the closest reference archetype from `references/reference-gallery.md` and explicitly adapt the image to that archetype rather than inventing a generic layout.
7. Build one minimal visual metaphor that supports the claim.
8. Apply Human 2.0 brand rules:
   - canvas `#F3F4F6`
   - white surfaces `#FFFFFF`
   - graphite text/lines `#2C2C2C`
   - primary indigo accent `#6366F1`
   - gold `#C4A148` only as a tiny secondary accent
   - modern clean sans-serif typography in the spirit of Onest/Geologica
   - calm, precise, practical, premium editorial tone
9. Generate the image with image generation when requested. Keep the final response concise: concept, headline, and any caveat about generated text/logo fidelity.

## Brand Language Rules

In Russian copy, write `ИИ`, not `AI`, except when `AI` is part of an official English name, quote, URL, citation, or unchanged product/standard name.

Use these brand names exactly:

- `Человек 2.0`
- `H2.0`
- `Среда внедрения ИИ`

Avoid:

- `Human20` as a public replacement for the brand name
- `H 2.0`
- `H-2.0`
- invented logos or distorted H2.0 badges

## Headline Rules

Use one large headline on the image, usually 2 lines for horizontal covers and 3-5 short lines for Reels. Make it feed-readable visually and semantically.

For Dzen, Telegram, Instagram, and other broad-audience covers, the headline should explain what the tool does or why the reader should care. A person unfamiliar with the tool should understand the value immediately.

Priority:

1. Clear user benefit
2. Real-world use case
3. Tool or product name
4. Technical proof
5. Implementation details

Prefer benefit-first headlines:

- `БЫСТРАЯ РАСШИФРОВКА АУДИО`
- `ЛОКАЛЬНАЯ ТРАНСКРИБАЦИЯ АУДИО`
- `ДЛИННЫЕ АУДИО БОЛЬШЕ НЕ НУЖНО ЖДАТЬ`
- `ВЫШЕЛ БЫСТРЫЙ WHISPER ДЛЯ GPU И MAC`
- `КАК БЫСТРО РАСШИФРОВАТЬ ДЛИННОЕ АУДИО`
- `АГЕНТСКИЙ КОДИНГ ТЕПЕРЬ СО СЧЁТЧИКОМ`
- `ПЛАГИНЫ ТЕПЕРЬ ЧИНЯТСЯ ОТДЕЛЬНО`
- `ОПЫТ - НОВОЕ ТОПЛИВО ИИ`
- `ОДНА ЗАПИСЬ - МНОГО ВИДЕО`
- `КУРСЫ ПО ИИ УСТАРЕВАЮТ БЫСТРЕЕ`
- `ВСЕ СООБЩЕСТВА ДОЛЖНЫ БЫТЬ AGENT FIRST`

Avoid as main headline for a broad audience:

- `WHISPER НА УСКОРЕНИИ`
- `ТРАНСКРИБАЦИЯ НА MPS`
- `FLASH ATTENTION ДЛЯ WHISPER`
- `CLI ДЛЯ BATCHING`
- restating the first sentence without sharpening it
- vague poetic lines that need the post to explain them
- long subtitles, tables, and tiny UI labels
- marketing mush such as `революция`, `будущее уже здесь`, `новая эра` unless the article itself truly argues that
- more than 5-7 generated words when exact Russian text fidelity is critical

Move technical details such as CLI, MPS, fp16, batching, Flash Attention, Transformers, Optimum, gateway, orchestration, or MCP into the article body or a small caption unless the user explicitly wants a technical cover.

If the user proposes a better headline, use it and regenerate rather than defending the previous line.

## Composition Rules

Default 16:9 structure: large headline on the left + one white rounded editorial panel or one focal object on the right + one continuous indigo path. Use at most 3-4 meaningful visual elements.

Signature Human 2.0 elements:

- Huge Geologica-like headline, black with 1 indigo accent word.
- White rounded panels with soft shadows.
- Thin indigo connector lines with small circular nodes.
- Small official H2.0 / Human 2.0 logo asset in the bottom-left safe zone.
- Optional 3x3 dot pattern in top-right or bottom-left.
- Tiny gold dot, spark, divider, or checkmark only as accent.
- Strong negative space and calm premium editorial layout.

Use these metaphors:

- route/control: nodes, switches, fallback paths, checkmarks
- long task durability: path, checkpoints, restore/gateway, finish mark
- agent tooling: schedule/clock -> tool chips -> result card
- usage economy: code/editor -> agent node -> credit meter
- media generation: chat -> tool tile/logo -> image/video cards
- avatar/content system: phone capture -> reusable presenter card -> small credit meter
- learning from experience: text pages fading -> board/action loop -> reward dot
- course vs living environment: crossed-out crown/course artifact -> living system/panel/environment
- community memory: chat stream -> structured memory -> agent-accessible skill cards

Avoid:

- dense before/after panels unless the user explicitly asks for a comparison infographic
- pricing tables
- benchmark grids
- many service logos
- subscription buttons
- emojis
- generic robot brain, cyberpunk, neon
- fake dense UI text
- huge green checkmarks
- cluttered infographic logic

## Logos, Mascots, And References

Use logos or mascots only when they materially improve recognition of the article topic.

Rules:

- Human 2.0 logos must come from official PNG/SVG assets from the brandbook at `human20.app/brand` or from attached official logo files.
- Do not ask the image model to invent, redraw, retype, stretch, or approximate the Human 2.0 logo.
- If no official logo asset is available, leave clean space for manual logo placement or use the plain text fallback `Человек 2.0 · Среда внедрения ИИ`.
- If the official logo is attached, preserve it exactly and place it as a composited asset in the bottom-left safe zone.
- If the user attaches a logo/mascot/image, use it as a reference and preserve its identity.
- If the user attaches strong visual references, treat them as the current quality bar and extract the layout pattern, typography scale, palette, spacing, and motif before generating.
- If no visual references are attached, use `references/reference-gallery.md` as the persistent internal reference library.
- If a current third-party logo is needed and not supplied, search the web for official brand assets or reliable visual references before prompting.
- Keep third-party logos small-to-medium and harmonized with Human 2.0. They should not dominate the cover unless the article is primarily about that brand.
- Never turn a comparison into an aggressive fight poster. Show the advantage through layout: open routes, fallback paths, control, completed result, or clean workflow.
- If editing an existing image, preserve the image content and frame it inside a Human 2.0 layout instead of redrawing it, unless the user asks for a new illustration.

## Image Prompt Template

Use this structure when calling image generation:

```text
Create a premium Human 2.0 branded <FORMAT> image for a Russian post/article about <topic>.

Format:
<16:9 Dzen/Telegram cover OR 9:16 Instagram/Reels cover OR 4:3/1:1 infographic>. Use safe margins and keep all important text away from edges.

Audience mode:
<Mass audience OR Editorial / expert OR Technical>. For mass audience, make the headline benefit-first and understandable to non-technical readers.

Reference archetype:
Use the closest archetype from references/reference-gallery.md: <archetype name>. Preserve its layout logic, hierarchy, spacing, and visual motifs while adapting the metaphor to this article.

Brand style:
Use Human 2.0 visual identity: light gray canvas #F3F4F6, white surfaces #FFFFFF, dark graphite typography and lines #2C2C2C, primary indigo accent #6366F1. Use gold #C4A148 only as a tiny secondary accent. Modern clean sans-serif typography similar to Onest/Geologica. Calm, precise, practical, premium editorial style.

Logo/footer:
Use the official attached Human 2.0 logo asset exactly as provided. Preserve its aspect ratio and place it in the bottom-left safe zone. If no official logo asset is available, leave clean space for manual logo placement or use only the plain text footer `Человек 2.0 · Среда внедрения ИИ`. Do not redraw or approximate the logo.

Core meaning:
<one paragraph explaining the article's main claim and why the reader should care>

Visual concept:
<one sparse metaphor with 3-4 elements max>

Composition:
<mode-specific composition from references/formats.md and references/generation-modes.md>. Use restrained indigo connectors/paths and tiny gold accent only where useful.

Text on image:
Use only this Russian headline, large and clean:
"<HEADLINE>"
Optional small caption only if there is enough space:
"<short product/topic caption>"

Style constraints:
Minimal premium editorial cover, crisp modern layout, subtle depth, generous spacing, restrained palette. No subscription button, no emojis, no cyberpunk, no neon, no fake dense UI text, no clutter, no watermark. In Russian text use "ИИ", not "AI", except official names or quoted terms.
```

## Refinement Workflow

When the user asks to fix a generated image:

1. Preserve the strongest existing composition unless the user asks to redesign.
2. Identify exactly what failed: text, logo, crop, visual density, brand mismatch, wrong format, or weak metaphor.
3. Use `references/anti-patterns.md` to prevent repeating the error.
4. For text fixes, reduce the amount of generated text or leave clean negative space for manual typography.
5. For logo fixes, use an official logo PNG/SVG from `human20.app/brand` or leave space for manual logo placement. Do not regenerate the logo from memory.
6. For crop fixes, extend canvas/outpaint rather than shrinking core content when the user asks not to change the infographic.

## Quality Check

Before finalizing, check the generated cover against these criteria:

- The headline is understandable without reading the post.
- For broad-audience covers, the practical benefit is clearer than the tool internals.
- The image communicates one idea, not a list of features.
- The palette reads Human 2.0, not purple SaaS, cyberpunk, or stock tech.
- Gold is a small accent, not the dominant look.
- Human 2.0 logo is either an official asset, a plain text fallback, or absent with clean space reserved for manual placement.
- The logo is not stretched, retyped, approximated, or distorted.
- Generated Russian text has no obvious spelling artifacts. If text is messy, regenerate with fewer words or no in-image text.
- The cover has no subscription button, fake tables, dense tiny labels, or visual clutter.
- Text is readable at thumbnail size.
- Critical text and brand marks sit inside the safe zone for the target format.
- The chosen reference archetype is visible in the layout, not just mentioned in the prompt.

## Evaluation Set

Use `references/evals.md` to test the skill on representative Human 2.0 tasks before major changes. A good version should produce images comparable to the user's references: clean, premium, branded, practical, and topic-specific.