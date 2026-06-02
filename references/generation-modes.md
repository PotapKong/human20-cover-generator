# Generation Modes

Choose one mode before prompting image generation.

## Minimal editorial cover

Use for articles, Dzen, Telegram, and most post covers.

Prompt emphasis:

- premium editorial cover
- finished GPT Image 2 cover, not a placeholder base
- bold Russian headline
- one metaphor
- clean product-slide composition
- real visual hook: object, rupture, glow, proof moment, or cinematic product surface
- no dense UI text
- Human 2.0 footer/badge
- not a reusable card-grid template

Good visual ideas:

- white panel with brand-blue route
- chat card -> agent node -> result card
- locked route vs open route
- document stack -> skill card
- control board with a single active path

First try to express the post as one hero object, real screenshot/evidence panel, or product surface. Use several cards only when they are the actual point of the story. Do not ask for empty right/left zones for later code layout unless doing a correction pass.

## Premium object cover

Use when user asks for `инстаграммная`, `крутая`, `вау`, `обложка`, cinematic, hyperrealistic, more premium visual weight, or when a normal article cover starts to look templated.

Prompt emphasis:

- one hyperrealistic object
- shallow depth of field
- soft blur and depth
- white/light-gray studio background
- brand blue and gold brand reflections
- abstract Human 2.0 UI elements around it
- bold editorial tension: breaking, opening, scanning, validating, routing, upgrading, or transforming
- no cyberpunk, no neon, no generic stock tech

Good objects:

- crown for `курс умер / да здравствует среда`
- iceberg for hidden AI capability
- glass robot + human for agent-first community
- notebook/grid for orchestrator or workflows
- control dial/panel for choosing routes
- white dashboard or monitor for product/tool posts
- polished document/artifact under search and AI citation beams for SEO/AI-answer posts

## Clean infographic

Use when user provides a table, chart, numbers, comparison, or existing rough infographic.

Prompt emphasis:

- redraw as editorial data card
- 2-4 data blocks max
- keep labels short
- use Human 2.0 palette
- avoid fake tiny numbers
- use large numbers and simple icons
- if data accuracy matters, keep visual labels minimal and do not invent extra values

## UI workflow diagram

Use only when the user asks for a process/workflow visual or when the article's main claim is the sequence itself. Do not use this mode merely because the topic includes agents, MCP, tools, automations, media generation, or skills.

Prompt emphasis:

- one continuous brand-blue route line
- white rounded panels
- 3-5 abstract tool cards
- small nodes and arrows
- no small unreadable code
- no fake detailed interface text
- must still have one dominant focal point, not equal-weight cards

Good flows:

- input material -> agent/tool -> output card
- chat -> gateway -> result cards
- brief -> agent -> skill -> final check

## Reels vertical cover

Use with `references/formats.md` 9:16 rules.

Prompt emphasis:

- strong headline top
- hero visual middle
- brand mark bottom
- safe margins for Instagram UI
- readable in grid crop
- no horizontal table or wide chart

## Refinement mode

Use when fixing a generated image.

Prompt emphasis:

- preserve existing composition
- change only requested element
- fix text/logo/crop/color without redesign
- for crop padding: outpaint clean background around existing content
- for text errors: reduce text or reserve manual typography space
