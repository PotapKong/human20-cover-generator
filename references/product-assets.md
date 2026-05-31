# Product Asset Rules

Use this file when a cover mentions a real product, company, tool, website, GitHub project, article, conference, or service.

## Core rule

Do not invent logos, product marks, mascots, website screenshots, dashboard screenshots, article screenshots, or UI fragments when the real source can be found.

Before generating a cover with recognizable products, collect the best available visual assets:

1. Official website or product page.
2. Official GitHub organization or repository.
3. Official docs.
4. User-provided screenshots or files.
5. Public article screenshot only when the cover is explicitly about that article or news item.

Use the official asset as a reference or composited image. Do not redraw it from memory.

## Search workflow

When a post mentions a product or tool:

1. Search the web for the official product/company page.
2. Search the official GitHub repo or organization when the tool is open source.
3. Search the official docs page if the logo is absent from the landing page.
4. Open the page and inspect visible images, screenshots, and logos.
5. If the exact logo cannot be obtained, use a text-only product card instead of a fake logo.

Recommended search patterns:

- product name + official site
- product name + GitHub
- product name + docs
- company name + official logo
- product name + official logo

## Screenshots

Screenshots are useful when:

- the article is about a specific website, product, repo, or news item
- the user asks to overlay or include a reference screenshot
- the product UI itself is the story
- the screenshot gives credibility to a news cover

Rules:

- Keep screenshots inside a rounded white card or browser frame.
- Crop to the meaningful part.
- Do not distort the aspect ratio.
- Do not cover the headline with screenshot details.
- If screenshot text is tiny or messy, blur or abstract it and keep only the recognizable composition.

## Known product mapping

### Hermes

When the user writes `Hermes`, `Hermes Agent`, or asks about Hermes in the agent/tooling context, treat it as:

- Product: `Hermes Agent`
- Organization: `Nous Research`
- Official Hermes Agent site: `hermes-agent.nousresearch.com`
- Parent site: `nousresearch.com`

Do not invent a winged H logo or generic Hermes icon. Use the real Hermes Agent / Nous Research visual identity from the official Hermes Agent page, the official Nous Research site, or a user-provided Hermes reference image.

If the official visual is not accessible, use a text-only card:

- `Hermes Agent`
- `by Nous Research`

and leave the logo area blank or use the user-provided reference.

### Human 2.0

Use official Human 2.0 assets from `human20.app/brand`. Do not redraw or approximate the H2.0 logo.

### Polymarket

Use official Polymarket brand assets from `polymarket.com/brand`.

Known official details:

- Brand page: `https://polymarket.com/brand`
- Logo pack: `https://polymarket-upload.s3.us-east-2.amazonaws.com/polymarket-logos.zip`
- Poly Blue: `#2E5CFF`
- Font direction: Inter

For Human 2.0 covers, keep Polymarket as a small official chip, market-question card, or entry-point badge inside the Human 2.0 layout. Do not let the Polymarket blue replace Human 2.0 indigo as the main accent.

If exact logo fidelity matters, download the logo pack and composite the official PNG/SVG after generation. If that is not possible, use a text-only card:

- `Polymarket`

Do not ask image generation to invent a Polymarket icon or redraw the wordmark from memory.

### Claude / Claude Code / Anthropic

Use official Anthropic / Claude pages and assets. If the exact logo cannot be obtained, use a text-only card:

- `Claude Code`
- `by Anthropic`

Do not invent a new Claude logo.

### Microsoft Copilot

Use official Microsoft pages and assets. If the exact logo cannot be obtained, use a text-only card:

- `Copilot`
- `by Microsoft`

Do not invent a new Copilot logo.

## Prompt wording

When official assets are available:

`Use the attached official product logo or screenshot exactly as provided. Preserve its aspect ratio. Do not redraw, retype, recolor, stretch, crop, or approximate it.`

When assets are not available:

`Use a clean text-only product card instead of a logo. Do not invent a fake logo.`

## Quality check

Before finalizing:

- Did every recognizable product mark come from an official or user-provided asset?
- If not, did we use a text-only fallback instead of a fake logo?
- Is Hermes treated as Hermes Agent by Nous Research?
- Are screenshots cropped and framed cleanly?
- Are there no fake UI labels pretending to be official product text?
