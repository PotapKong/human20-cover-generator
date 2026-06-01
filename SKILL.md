---
name: human20-cover-generator
description: Create premium Human 2.0 branded article, Telegram, Dzen, Instagram/Reels, and social cover images from a post/article text. Use when the user asks to придумать/сгенерировать/перегенерировать баннер, обложку, картинку, cover, image, illustration, инфографику, vertical reels cover, or заменить перегруженную инфографику for a text; when they want a short Russian headline on the image; when they mention Human 2.0 brand style, brandbook, logos, mascots, GPT Image, or fitting a provided image/logo into a clean Human 2.0 layout.
---

# Human 2.0 Cover Generator

## Overview

Turn article/post text into a premium, juicy, editorial Human 2.0 cover. Prefer one clear idea, one short headline, one strong metaphor, and a bold generated visual over dense infographics or code-built layouts.

If the user asks to generate immediately, use the built-in image generation flow after shaping the concept. Do not stop at a prompt unless the user asks only for a prompt.

## Generative-First Rule

GPT Image 2 should create the actual cover art and composition: hero object, lighting, depth, particles, soft UI surfaces, route lines, icons, and overall atmosphere. Do not replace image generation with a PIL/HTML/SVG reconstruction of the cover. Code/manual compositing is allowed only for narrow production fixes:

- overlay the official Human 2.0 logo asset if the generated logo is wrong;
- replace or sharpen the exact headline if Russian text fidelity fails;
- insert a real screenshot when the screenshot itself is the requested evidence.

Never use code to draw the main composition, cards, panels, shadows, icons, or "template base" unless the user explicitly asks for a deterministic infographic. If a generated cover feels weak, regenerate with a stronger concept instead of assembling a safe layout manually.

## Generation Feedback Loop

Use this loop for every production cover:

1. Generate a finished GPT Image 2 cover from the chosen Reference DNA archetype.
2. Inspect it against `references/reference-dna.md` and the Quality Check below.
3. If the result is generic, card-heavy, low-energy, or has no dominant hero/proof, regenerate with a stronger object/evidence concept.
4. If only the logo, exact headline, or exact screenshot is wrong, make a narrow production fix using the official asset or real screenshot.
5. Do not turn a weak generation into a final cover by rebuilding it in code.

## Mandatory Reference Intake

Before calling image generation or writing a final image prompt, you MUST complete a reference intake. Do not rely only on the summary in this `SKILL.md`.

Always read these reference files for new cover generation:

- `references/reference-dna.md`
- `references/headline-patterns.md`
- `references/reference-gallery.md`
- `references/visual-system.md`
- `references/typography-lock.md`
- `references/accent-colors.md`
- `references/formats.md`
- `references/generation-modes.md`

Read these conditionally:

- `references/logo-assets.md` before adding any Human 2.0 logo or footer.
- `references/product-assets.md` before adding third-party logos, product screenshots, website screenshots, GitHub screenshots, or article screenshots.
- `references/anti-patterns.md` before refinement, when text/logo/color fidelity matters, or when a previous generation missed the style.
- `references/cover-patterns.md` when choosing between concepts or improving a weak metaphor.

If `references/images/` contains examples relevant to the requested format or topic, inspect 3-5 closest image files with the available visual tool before prompting. Use fewer only when fewer relevant examples exist or visual inspection is unavailable. If a file name starts with `TOP Reference`, inspect it first and treat it as the primary style benchmark unless the user explicitly asks for a different format. Extract the layout pattern, typography scale, palette, spacing, motif, density, and where the examples intentionally break the default card pattern. If the user supplies fresh typography references, treat those references as the active quality bar and apply `references/typography-lock.md` over generic bundled typography wording. If visual inspection is unavailable, say that briefly and use `references/reference-gallery.md` as the fallback.

Before image generation, name the reference intake in your working notes or prompt plan:

- audience mode
- generation mode
- selected reference archetype
- whether `TOP Reference` was used, and if not, why
- selected Reference DNA archetype
- 3-5 visible traits copied from the references or gallery
- typography rule, including whether user-supplied references override the default condensed class
- palette rule
- anti-patterns being actively avoided

Do not call image generation if you cannot name the selected archetype and at least 3 concrete visual traits from the inspected references. If `TOP Reference` exists and was skipped, do not generate until you can state a concrete reason.

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
4. Complete the Mandatory Reference Intake above before prompting.
5. Choose one short Russian headline that is understandable in a feed. For broad-audience covers, lead with benefit or use case, not tool internals.
6. Choose the closest reference archetype from `references/reference-gallery.md` and explicitly adapt the image to that archetype rather than inventing a generic layout.
7. Build one minimal visual metaphor that supports the claim.
8. Choose the Reference DNA archetype from `references/reference-dna.md`.
9. Apply Human 2.0 brand rules:
   - canvas `#F3F4F6`
   - white surfaces `#FFFFFF`
   - graphite text/lines `#2C2C2C`
   - primary indigo accent `#6366F1`
   - gold `#C4A148` only as a tiny secondary accent
   - reference-matched heavy condensed display typography for the main headline, with Onest/Geologica only for captions and brand support text
   - official Human 2.0 mascot from `references/images/maskot.jpg` as a small brand companion when available
   - calm, precise, practical, premium editorial tone
10. Generate the image with GPT Image 2 / built-in image generation when requested. Keep the final response concise: concept, headline, and any caveat about generated text/logo fidelity.

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

Default 16:9 structure: large headline + one strong generated visual answer: either a hyperreal/editorial hero object, a cinematic product scene, a framed real screenshot/evidence moment, or one concise product surface. Add a continuous indigo path only when it clarifies the idea. Use at most 3-4 meaningful visual elements.

Do not default to a repeated right-side workflow/card block just because the article mentions processes, tools, or skills. Use that structure only when the inspected references support it for the specific topic. If `TOP Reference` is present, prefer its premium editorial object/hero rhythm over a generic card grid: expressive headline, one strong object or framed evidence, controlled depth, and sparse supporting icons.

### Anti-Template Lock

Before prompting GPT Image, choose the thumbnail hook in this order:

1. A strong editorial object/metaphor from the article.
2. A real screenshot or product evidence framed as the hero.
3. A single product/workspace panel.
4. A workflow/card diagram only if the user asks for process visualization or the inspected reference clearly uses that structure.

If the first prompt idea is `white panel + 4 cards + connector line`, reject it unless there is a concrete reason it will be more clickable than a hero object or framed evidence. For GPT Image 2, prompt a finished cover, not an empty placeholder scene. Reserve manual compositing only as a correction step after generation, not as the default design method.

### Juicy Cover Standard

The best Human 2.0 covers feel like editorial posters, not SaaS wireframes. A strong result usually has:

- one thumb-stopping object or product scene with depth, gloss, rupture, light, material contrast, or motion;
- a huge reference-matched condensed headline that dominates the feed without looking vertically stretched;
- Human 2.0 white/indigo/gold system elements integrated into the scene, not pasted as decoration;
- small supporting UI icons/cards only as satellites around the hero, never as the main content by default;
- visible tension from the article: broken old habit, opened route, controlled pipeline, finished artifact, warning state, or upgrade moment.

If the image could be reused for ten unrelated AI posts by only changing the headline, reject the concept and regenerate.

### Reference DNA Lock

After inspecting the user/repo references, map the cover to one of `references/reference-dna.md`:

- Broken Old Model / Crown
- Premium Device / Agent Inside
- Evidence Collage
- Real Screen Hero
- Before / After Product Outcome

Do not generate until the prompt names one of these and describes the dominant proof/hero. When the topic is about a repo, article, benchmark, conference, audit, or public claim, prefer `Evidence Collage` or `Real Screen Hero` over a generic workflow.

Signature Human 2.0 elements:

- Huge heavy condensed display headline, black with 1 indigo accent word.
- White rounded panels with soft shadows.
- Thin indigo connector lines with small circular nodes.
- Small official H2.0 / Human 2.0 logo asset in the bottom-left safe zone.
- Optional 3x3 dot pattern in top-right or bottom-left.
- Tiny gold dot, spark, divider, or checkmark only as accent.
- Strong negative space and calm premium editorial layout.

Typography and color must match the reference system closely:

- Match the headline font class, proportions, line rhythm, and spacing from the inspected or user-supplied references. Current premium references use a heavy condensed poster/display grotesk: tall compact glyphs, tight line-height, hard vertical strokes, minimal roundness, and enough width for thumbnail readability.
- Do not interpret `condensed` as permission to vertically stretch or make needle-thin letters. If the headline looks like ultra-condensed vertical bars or is about 1.25x taller/narrower than the active reference, reject it.
- Do not default to `Geologica.ttf` for the main headline when references show this condensed poster style. Geologica is too wide/soft for those covers and is only a fallback for non-reference work.
- If rendering typography manually and no exact reference font is bundled, prefer an available licensed heavy condensed Cyrillic display face with comparable proportions over Geologica/Arial Narrow. If exact fidelity is required, stop and ask for or source the exact display font asset.
- Use graphite `#2C2C2C` for dark headline words and `#6366F1` for the single indigo accent phrase.
- If rendering secondary brand text manually, use the bundled `assets/brand/Geologica.ttf` or `assets/brand/Onest.ttf` where appropriate.
- Do not let screenshots or generated gradients drift the overall palette away from the Human 2.0 reference.

### Headline Font Consistency Lock

For every Dzen / Telegram / horizontal Human 2.0 cover:

1. Inspect the supplied/user/exported references and name the headline font class before rendering.
2. If user-supplied typography references are present, they override generic bundled wording. The main headline must match their visible proportions, line height, left spacing, and black/indigo rhythm.
3. Preferred durable asset order:
   - exact user-provided or repo-bundled licensed display font, such as `assets/brand/h20-display-condensed.ttf` if present;
   - an available licensed heavy condensed Cyrillic display face with comparable proportions;
4. When exact Russian text and brand typography matter, first try a short generated headline in the GPT Image cover. If it fails, replace only the headline in a narrow correction pass while preserving the generated design.
5. Final quality gate: compare the headline against the closest reference. If letters are too wide, too rounded, too soft, too narrow, too tall, vertically stretched, or the line rhythm looks unlike the reference poster grotesk, reject and rerender typography before final delivery.

Use these metaphors as starting points, but turn them into one decisive cover image rather than a generic diagram:

- route/control: nodes, switches, fallback paths, checkmarks
- long task durability: path, checkpoints, restore/gateway, finish mark
- agent tooling: schedule/clock -> tool chips -> result card
- usage economy: code/editor -> agent node -> credit meter
- media generation: chat -> tool tile/logo -> image/video cards
- avatar/content system: phone capture -> reusable presenter card -> small credit meter
- learning from experience: text pages fading -> board/action loop -> reward dot
- course vs living environment: crossed-out crown/course artifact -> living system/panel/environment
- community memory: chat stream -> structured memory -> agent-accessible skill cards
- SEO / AI-search article pipeline: a finished article artifact being scanned by search/AI beams, a polished document moving through verification gates, or a browser/repo evidence panel orbiting one hero document; avoid a flat checklist of cards

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

## Logos, Mascots, Screenshots, And References

Use logos, mascots, screenshots, or website/article captures only when they materially improve recognition or credibility of the cover.

Rules:

- For Human 2.0 covers, include the official mascot by default when `references/images/maskot.jpg` is available, unless the user explicitly asks not to or the format would make it unreadable.
- Prefer using the official mascot asset as a final composited overlay when exact identity matters. If GPT Image 2 invents or distorts the mascot, replace it with the official asset.
- Place the mascot as a small brand companion near the hero object, route node, product panel, or proof chip. Do not let it compete with the headline, logo, or main proof.
- Human 2.0 logos must come from official PNG/SVG assets from the brandbook at `human20.app/brand` or from attached official logo files.
- If local official assets exist in `assets/brand/`, use them before falling back to plain text. Preferred horizontal cover asset: `assets/brand/h20-lockup-dark-1440.png` or `assets/brand/h20-lockup-dark.svg`.
- Do not ask the image model to invent, redraw, retype, stretch, or approximate the Human 2.0 logo.
- When exact logo fidelity matters, generate the cover with clean space for the logo and composite the official PNG/SVG asset after generation. Prompt-only logo recreation is not enough for final production.
- If no official Human 2.0 asset is available, leave clean space for manual logo placement or use the plain text fallback `Человек 2.0 · Среда внедрения ИИ`.
- For every named third-party product, platform, market, repository, or company that appears in the article or requested cover, read `references/product-assets.md` and check official sources before deciding whether to use a logo, product chip, screenshot, or text-only fallback.
- Third-party logos and product marks must come from official websites, official docs, official GitHub repositories, official social/profile assets, or user-provided reference files.
- When exact third-party logo fidelity matters, use the official PNG/SVG as a final composited overlay or use a text-only product card. Do not rely on image generation to redraw the logo.
- When the user mentions `Hermes`, `Hermes Agent`, or Hermes in the agent/tooling context, treat it as `Hermes Agent` by `Nous Research`. Use `hermes-agent.nousresearch.com`, `nousresearch.com`, or user-provided Hermes references as the visual source. Do not invent a winged H logo or generic Hermes mark.
- If the official third-party logo cannot be obtained, use a clean text-only product card instead of a fake logo.
- If the user asks to overlay a reference screenshot or article screenshot, frame it inside a rounded white card/browser frame, crop only to the meaningful area, and preserve its aspect ratio.
- If the user attaches a logo/mascot/image/screenshot, use it as a reference and preserve its identity.
- If the user attaches strong visual references, treat them as the current quality bar and extract the layout pattern, typography scale, palette, spacing, and motif before generating.
- If no visual references are attached, use `references/reference-gallery.md` as the persistent internal reference library.
- If a current third-party logo or screenshot is needed and not supplied, search the web for official brand assets, product pages, docs, GitHub pages, and reliable visual references before prompting.
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

Reference DNA:
Use the closest archetype from references/reference-dna.md: <Broken Old Model / Crown OR Premium Device / Agent Inside OR Evidence Collage OR Real Screen Hero OR Before / After Product Outcome>. The dominant hero/proof is <one sentence>. Supporting cards/icons are satellites only.

Reference evidence:
Use these concrete traits from the 3-5 inspected references or gallery: <3-5 traits covering layout, typography scale, spacing, palette, motif, visual density, and whether the right-side visual should be a workflow, large screen, object, or mixed panel>.

Asset sources:
Use official or user-provided assets for all recognizable logos, product marks, mascots, website screenshots, GitHub screenshots, and article screenshots. For Human 2.0 covers, use `references/images/maskot.jpg` as the official mascot asset when available and keep its `human20.app` screen readable. If the product is Hermes, use Hermes Agent by Nous Research as the source, not a generic Hermes mark. If an official asset is unavailable, use a text-only product card and do not invent a fake logo.

Brand style:
Use Human 2.0 visual identity: light gray canvas #F3F4F6, white surfaces #FFFFFF, dark graphite typography and lines #2C2C2C, primary indigo accent #6366F1. Use gold #C4A148 only as a tiny secondary accent. Do not use green as an accent except inside preserved real screenshots. Main headline typography must match the active reference proportions; for current premium references this means a heavy condensed poster/display grotesk with natural Cyrillic width, not Geologica and not vertically stretched ultra-condensed text. Use Onest/Geologica only for captions, brand support text, and secondary UI-like labels. Calm, precise, practical, premium editorial style.

Logo/footer:
Use the official attached Human 2.0 logo asset exactly as provided. Preserve its aspect ratio and place it in the bottom-left safe zone. If no official logo asset is available, leave clean space for manual logo placement or use only the plain text footer `Человек 2.0 · Среда внедрения ИИ`. Do not redraw or approximate the logo.

Core meaning:
<one paragraph explaining the article's main claim and why the reader should care>

Visual concept:
<one sparse metaphor with 3-4 elements max>

Composition:
<mode-specific composition from references/formats.md and references/generation-modes.md>. Make this a finished GPT Image 2 cover, not a blank base for later layout. Use restrained indigo connectors/paths and tiny gold accent only where useful.

Text on image:
Use only this Russian headline, large and clean:
"<HEADLINE>"
Optional small caption only if there is enough space:
"<short product/topic caption>"

Style constraints:
Premium editorial cover, juicy but restrained, crisp modern layout, strong depth/materiality, generous spacing, restrained palette. No placeholder composition, no blank text zones, no subscription button, no emojis, no cyberpunk, no neon, no fake dense UI text, no clutter, no watermark. In Russian text use "ИИ", not "AI", except official names or quoted terms.
```

## Refinement Workflow

When the user asks to fix a generated image:

1. Preserve the strongest existing composition unless the user asks to redesign.
2. Identify exactly what failed: text, logo, crop, visual density, brand mismatch, wrong format, or weak metaphor.
3. Use `references/anti-patterns.md` to prevent repeating the error.
4. For text fixes, reduce the amount of generated text or leave clean negative space for manual typography.
5. For Human 2.0 logo fixes, use an official logo PNG/SVG from `human20.app/brand` or leave space for manual logo placement. Do not regenerate the logo from memory.
6. For third-party logo fixes, search the official source or use a user-provided asset. If the asset cannot be verified, replace the fake logo with a text-only product card.
7. For screenshot fixes, crop/frame the real screenshot instead of recreating it as fake UI.
8. For crop fixes, extend canvas/outpaint rather than shrinking core content when the user asks not to change the infographic.

## Quality Check

Before finalizing, check the generated cover against these criteria:

- Mandatory Reference Intake was completed before generation.
- `references/reference-dna.md` was applied and the selected DNA archetype is visible.
- The selected reference archetype and 3 concrete visual traits are visible in the result, not just mentioned in the prompt.
- The headline font class, width/height ratio, line rhythm, and margins match the inspected or user-supplied reference; the final headline is not Geologica, Onest, Arial, Arial Narrow, Inter, Segoe UI, or vertically stretched ultra-condensed text when the reference uses the Human 2.0 poster style.
- The headline is understandable without reading the post.
- For broad-audience covers, the practical benefit is clearer than the tool internals.
- The image communicates one idea, not a list of features.
- GPT Image produced the main visual/composition. Manual code was not used to construct the cover, except for narrow logo/headline/screenshot correction.
- The cover has a thumb-stopping hook: hero object, cinematic product scene, framed proof moment, or strong visual tension.
- The result would not look like a generic reusable AI-template if the headline were swapped.
- Cards/routes/icons are satellites around the hero unless the user asked for a workflow diagram.
- The palette reads Human 2.0, not purple SaaS, cyberpunk, or stock tech.
- Custom accents are indigo/blue `#6366F1`, not green/lime.
- Gold is a small accent, not the dominant look.
- Human 2.0 mascot from `references/images/maskot.jpg` is present as a small brand companion when available, unless explicitly excluded or visually unsuitable.
- Human 2.0 logo is either an official asset, a plain text fallback, or absent with clean space reserved for manual placement.
- Third-party logos are official/user-provided assets or replaced with text-only cards.
- Any logo that must be exact was composited from an official asset after generation, or clean space was reserved for manual placement.
- If Hermes is mentioned, it is represented as Hermes Agent by Nous Research, not a fake generic Hermes logo.
- The logo is not stretched, retyped, approximated, or distorted.
- Screenshots are real/user-provided/officially sourced, cropped cleanly, and framed without distortion.
- Generated Russian text has no obvious spelling artifacts. If text is messy, regenerate with fewer words or no in-image text.
- The cover has no subscription button, fake tables, dense tiny labels, or visual clutter.
- Text is readable at thumbnail size.
- If typography was composited manually, the final response or working notes name the headline font used.
- Critical text and brand marks sit inside the safe zone for the target format.
- The chosen reference archetype is visible in the layout, not just mentioned in the prompt.

## Evaluation Set

Use `references/evals.md` to test the skill on representative Human 2.0 tasks before major changes. A good version should produce images comparable to the user's references: clean, premium, branded, practical, and topic-specific.
