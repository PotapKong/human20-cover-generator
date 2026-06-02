# Human 2.0 Cover Patterns

Use this reference when a post needs a stronger visual metaphor or when a generated cover feels too generic.

## Editorial Extraction

Convert the article into this internal brief:

- Topic: product, release, trend, comparison, or warning.
- Claim: what changed or what the author believes.
- Reader consequence: what the reader should do differently.
- Tension: convenience vs control, fixed price vs meter, chat answer vs real work, one-off tool vs workflow layer.
- Visual metaphor: one object/path/panel that shows the consequence.
- Thumbnail hook: why this image would stop scrolling before the reader reads the small text.

Do not visualize all facts. Visualize the decision the reader should remember.

## Generative Direction

Use GPT Image 2 to make the full cover feel alive. Prompt for the finished poster: lighting, depth, material, motion, evidence, headline hierarchy, and Human 2.0 accents together. Do not prompt a sterile base with empty zones unless you are only fixing text/logo after a failed generation.

When the result looks like an old template, increase the concept before increasing the number of UI elements:

- add one physical or semi-physical hero object;
- show transformation, rupture, scan, validation, route opening, or completion;
- make a real screenshot/evidence panel a secondary proof point, not the whole design;
- keep cards/icons as satellites around the object.

## TOP Reference Priority

When a premium Dzen / Telegram cover feels too generic, return to the `TOP Reference` image in `references/images/` before inventing a new structure.

The TOP Reference favors:

- one memorable editorial object or framed proof point
- expressive headline treatment
- sparse supporting icons
- Human 2.0 logo used exactly
- strong depth and material contrast where appropriate
- generated visual energy: particles, reflections, soft glow, blur, motion, or tactile object detail used with restraint

It does not favor repeating the same right-side workflow/card block for every post. Use workflow cards only when they are the actual metaphor, not as a default layout.

## Headline Patterns

Good Human 2.0 cover headlines are concrete and slightly compressed:

- `<THING> ТЕПЕРЬ <PRACTICAL CONSEQUENCE>`
- `<SYSTEM> БЕЗ <PAIN>`
- `<ACTION> С <NEW CONSTRAINT>`
- `<OLD HABIT> УХОДИТ, <NEW SKILL> ОСТАЁТСЯ`
- `<PRODUCT/RELEASE> ЧИНИТ <MAIN WORKFLOW>`

Avoid headlines that require prior context:

- `ПРОСНУЛСЯ С ИНСТРУМЕНТАМИ`
- `НОВЫЙ СЛОЙ РАБОТЫ`
- `БУДУЩЕЕ УЖЕ ЗДЕСЬ`

Use direct product names when recognition matters:

- `OPENCLAW VS CLAUDE CODE`
- `В OPENCLAW 5.4 ПОЧИНИЛИ АВТОЗАПУСК`
- `HIGGSFIELD MCP`

## Common Topics

### Release/update posts

Visual: one clean product scene with the fixed workflow, or a hero object that signals the update. Avoid equal-weight cards unless they are the story.

Examples:
- schedule -> tools -> result
- plugin tiles -> separate repair indicators -> gateway block
- health input -> status check -> alert

Headline style:
- `В OPENCLAW 5.4 ПОЧИНИЛИ АВТОЗАПУСК`
- `ПЛАГИНЫ ТЕПЕРЬ ЧИНЯТСЯ ОТДЕЛЬНО`
- `АГЕНТ НЕ МОЛЧИТ НЕЗАМЕТНО`

### Agent/runtime durability

Visual: long path with checkpoints, restore symbol, final check; make the path feel physical or cinematic, not a flat diagram.

Headline style:
- `ЗАДАЧА ДОЛЖНА ДОЙТИ ДО КОНЦА`
- `ДЛИННЫЕ ЗАДАЧИ ПЕРЕЖИВАЮТ СБОИ`

### Pricing/economics

Visual: code/editor -> agent node -> restrained meter/gauge. No coin piles.

Headline style:
- `АГЕНТСКИЙ КОДИНГ ТЕПЕРЬ СО СЧЁТЧИКОМ`
- `ТОП-МОДЕЛИ НУЖНО МАРШРУТИЗИРОВАТЬ`

### Closed vs open control

Visual: closed box with one locked route vs open routing panel with fallback paths.

Headline style:
- `OPENCLAW VS CLAUDE CODE`
- `КОНТРОЛЬ НАД СТЕКОМ ВАЖНЕЕ УДОБНОГО ВХОДА`

### Media tools/MCP

Visual: agent chat -> branded tool tile -> image/video output cards.

Headline style:
- `МЕДИА ВНУТРИ АГЕНТА`
- `АГЕНТ САМ СОБИРАЕТ МЕДИА`

### AI avatars/content production

Visual: phone capture -> reusable presenter card -> subtle credit marker.

Headline style:
- `ОДНА ЗАПИСЬ - МНОГО ВИДЕО`
- `ВИДЕОПРЕЗЕНТЕР БЕЗ ПЕРЕСЪЁМКИ`

### AI learning from experience

Visual: fading text pages -> board/action loop -> reward dot.

Headline style:
- `ОПЫТ - НОВОЕ ТОПЛИВО ИИ`
- `ИИ УЧИТСЯ НЕ ТОЛЬКО НА ТЕКСТАХ`

### Historical analogy

If user provides a detailed historical/illustrative image, do not replace it with a generic generated scene. Frame it in Human 2.0 layout and add a sharp headline.

Example:
- `МЕНЬШЕ ЧЕЛНОКА, БОЛЬШЕ КОНТРОЛЯ`

### SEO / AI-answer publishing

Visual: one finished article/document artifact or browser page being scanned, cited, and validated by Google/search and ИИ-answer signals. A real GitHub/README screenshot can appear as a small framed proof point. Avoid turning the cover into a pipeline diagram with `plan/article/schema/review` cards.

Headline style:
- `БЛОГ ПОД GOOGLE И ИИ-ОТВЕТЫ`
- `СТАТЬЯ, КОТОРУЮ МОЖНО ПРОВЕРИТЬ`
- `SEO-ТЕКСТ БЕЗ РУЧНОГО ХАОСА`

## Prompt Details That Help

Add these constraints when the generator overcomplicates:

- "Use only 3 main visual elements."
- "No before/after boxes."
- "No dense UI text, only abstract bars."
- "No subscription button."
- "No pricing table or benchmark table."
- "Use one continuous brand-blue route line."
- "Keep the brand logo small and integrated."
- "The image should feel like a premium editorial cover, not a product infographic."

For in-image Russian text, fewer words are safer. If the model misspells Russian, generate without text and leave negative space for manual typography.
