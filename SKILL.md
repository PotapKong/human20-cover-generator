---
name: human20-cover-generator
description: Create minimalist Human 2.0 branded article, Telegram, Dzen, and social cover images from a post/article text. Use when the user asks to придумать/сгенерировать/перегенерировать баннер, обложку, картинку, cover, image, illustration, or заменить перегруженную инфографику for a text; when they want a short Russian headline on the image; when they mention Human 2.0 brand style, brandbook, logos, mascots, or fitting a provided image/logo into a clean Human 2.0 layout.
---

# Human 2.0 Cover Generator

## Overview

Turn article/post text into a minimal, editorial Human 2.0 cover. Prefer one clear idea, one short headline, one visual metaphor, and a restrained brand-system composition over dense infographics.

If the user asks to generate immediately, use the built-in image generation flow after shaping the concept. Do not stop at a prompt unless the user asks only for a prompt.

## Core Workflow

1. Read the supplied text and extract the central editorial claim, not every detail.
2. Choose one short Russian headline that is understandable in a feed. Prefer concrete wording over poetic ambiguity.
3. Build one minimal visual metaphor that supports the claim.
4. Apply Human 2.0 brand rules:
   - canvas `#F3F4F6`
   - white surfaces `#FFFFFF`
   - graphite text/lines `#2C2C2C`
   - primary indigo accent `#6366F1`
   - gold `#C4A148` only as a tiny secondary accent
   - modern clean sans-serif typography in the spirit of Onest/Geologica
   - calm, precise, practical, premium editorial tone
5. Use a horizontal `16:9` cover by default for Dzen/Telegram/social feeds.
6. Generate the image with `image_gen` when requested. Keep the final response concise: headline, metaphor, and any caveat about generated text/logo fidelity.

## Headline Rules

Use one large headline on the image, usually 2 lines. Make it feed-readable and tied to the article's practical consequence.

Prefer:
- `АГЕНТСКИЙ КОДИНГ ТЕПЕРЬ СО СЧЁТЧИКОМ`
- `ПЛАГИНЫ ТЕПЕРЬ ЧИНЯТСЯ ОТДЕЛЬНО`
- `В OPENCLAW 5.4 ПОЧИНИЛИ АВТОЗАПУСК`
- `ОПЫТ - НОВОЕ ТОПЛИВО ИИ`
- `ОДНА ЗАПИСЬ - МНОГО ВИДЕО`

Avoid:
- restating the first sentence without sharpening it
- vague poetic lines that need the post to explain them
- long subtitles, tables, and tiny UI labels
- marketing mush such as "революция", "будущее уже здесь", "новая эра" unless the article itself truly argues that

If the user proposes a better headline, use it and regenerate rather than defending the previous line.

## Composition Rules

Default structure: large headline + one white rounded editorial panel + one continuous indigo path or focal object. Use at most 3-4 meaningful visual elements.

Use these metaphors:
- route/control: nodes, switches, fallback paths, checkmarks
- long task durability: path, checkpoints, restore/gateway, finish mark
- agent tooling: schedule/clock -> tool chips -> result card
- usage economy: code/editor -> agent node -> credit meter
- media generation: chat -> tool tile/logo -> image/video cards
- avatar/content system: phone capture -> reusable presenter card -> small credit meter
- learning from experience: text pages fading -> board/action loop -> reward dot

Avoid:
- dense before/after panels
- pricing tables
- benchmark grids
- many service logos
- subscription buttons
- emojis
- robots, generic AI brain, cyberpunk, neon
- fake dense UI text
- huge green checkmarks
- cluttered infographic logic

## Logos, Mascots, And References

Use logos or mascots only when they materially improve recognition of the article topic.

Rules:
- If the user attaches a logo/mascot/image, use it as a reference and preserve its identity.
- If a current logo is needed and not supplied, search the web for official brand assets or reliable visual references before prompting.
- Keep third-party logos small-to-medium and harmonized with Human 2.0. They should not dominate the cover unless the article is primarily about that brand.
- Never turn a comparison into an aggressive fight poster. Show the advantage through layout: open routes, fallback paths, control, completed result, or clean workflow.
- If editing an existing image, preserve the image content and frame it inside a Human 2.0 layout instead of redrawing it, unless the user asks for a new illustration.

## Image Prompt Template

Use this structure when calling image generation:

```text
Create a minimalist Yandex Zen / Telegram article cover image in the Human 2.0 brand style for a Russian post about <topic>.

Format:
Horizontal 16:9 social/news cover, readable in feed, clean and minimal.

Brand style:
Use Human 2.0 visual identity: light gray canvas #F3F4F6, white surfaces #FFFFFF, dark graphite typography and lines #2C2C2C, primary indigo accent #6366F1. Use gold #C4A148 only as a tiny secondary accent. Modern clean sans-serif typography similar to Onest/Geologica. Calm, precise, practical, premium editorial style.

Core meaning:
<one paragraph explaining the article's main claim and why the reader should care>

Visual concept:
<one sparse metaphor with 3-4 elements max>

Composition:
Large headline with generous negative space. One clean white rounded panel. Use restrained indigo connectors/paths and tiny gold accent only where useful. Avoid dense infographic structure.

Text on image:
Use only this Russian headline, large and clean:
"<HEADLINE>"
Small subtle caption, optional:
"<short product/topic caption>"

Style constraints:
Minimal vector-like editorial illustration, flat shapes, crisp edges, subtle depth, generous spacing, restrained palette. No subscription button, no emojis, no robots, no cyberpunk, no neon, no fake dense UI text, no clutter, no watermark.
```

## Quality Check

Before finalizing, check the generated cover against these criteria:

- The headline is understandable without reading the post.
- The image communicates one idea, not a list of features.
- The palette reads Human 2.0, not purple SaaS, cyberpunk, or stock tech.
- Gold is a small accent, not the dominant look.
- Any logos/mascots are recognizable but integrated.
- Generated Russian text has no obvious spelling artifacts. If text is messy, regenerate with fewer words or no in-image text.
- The cover has no subscription button, fake tables, dense tiny labels, or visual clutter.

For detailed reusable patterns and examples, read [references/cover-patterns.md](references/cover-patterns.md) only when choosing between several concepts or refining a failed generation.
